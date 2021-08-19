<script>
  import { link } from "svelte-routing";

  // core components
  const nimLogo = "/android-chrome-512x512.png"

</script>

<svelte:head>
  <title>Nim Wiki - Directory</title>
</svelte:head>


<section class="relative flex h-screen bg-secondary-dark bg-no-repeat">
  <a
    href="/"
    class="absolute top-0 left-0 max-w-150-px"
    style="margin-left: 50px; margin-top: 50px;"
  >
    <img
      src="{nimLogo}"
      alt="Nim Wiki Logo"
    />
  </a>
    
  <div class="container mx-auto grid justify-items-center max-h-860-px">
    <h2 class="font-semibold text-4xl text-primary mt-48">
      Domain directory
    </h2>

    <div class="flex items-baseline justify-between w-full max-w-6xl">
      <span class="text-2xl text-primary mr-4">
        <a
          href="https://demo.nim.wiki"
          class="text-primary font-bold"
          target="_blank"
        >
          demo.nim.wiki
        </a>
      </span>

      <span class="text-xl text-white ml-4">
        A demo GitHub Pages project using a basic template to show what the result would be like.
      </span>
      
    </div>

   

  </div>
</section>
