<!-- App.svelte -->
<script>
  import { Router, Route } from "svelte-routing";

  // No Layout Pages
  import Index from "./views/Index.svelte";
  import Apply from "./views/Apply.svelte";
  import Directory from "./views/Directory.svelte";

  export let url = "";
</script>

<Router url="{url}">
  <!-- no layout pages -->
  <Route path="/" component="{Index}" />
  <Route path="/apply" component="{Apply}" />
  <Route path="/directory" component="{Directory}" />

</Router>
