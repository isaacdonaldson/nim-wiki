<script>
  import { fade } from 'svelte/transition';

  //TODO navigating away needs fadout to happen


  export let words;
  export let classStyle = "text-white"

  let visible = true
  let showWord = true
  let idx = 0

  //Make the cursor pulse visibility
  setInterval(() => (visible = !visible), 500)

  const sleep = (ms) => {
    return new Promise(resolve => setTimeout(resolve, ms));
  }

  function typewriterIn(node, { speed = 100 }) {
    const text = words[idx]
    const duration = text.length * speed;

    return {
      duration,
      tick: t => {
        const i = ~~(text.length * t);
        node.textContent = text.slice(0, i);
        if(t == 1){
          sleep(1500).then(() => {
            showWord = false
          })
        }
      }
    };
  }

   function typewriterOut(node, { speed = 100 }) {
    const text = words[idx]
    const duration = 1

    return {
      duration,
      tick: t => {
        const i = ~~(text.length * t);
        node.textContent = text.slice(0, i);
        if(t == 0) {
          sleep(500).then(() => {
            if (idx + 1 >= words.length ) {
              idx = 0
            } else {
              idx = idx + 1
            }
            showWord = true
          })
        }
      }
    };
  }
</script>



<div class="flex flex-row">
  {#if showWord}
  <div in:typewriterIn out:typewriterOut class="{classStyle}">
    {words}
  </div>
  {/if}

  {#if visible}
  <p class="{classStyle}">|</p>
  {/if}

</div>
