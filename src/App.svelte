<script>
  import { Router, Route } from "svelte-routing";
  import Navbar from "./components/Navbar.svelte";
  import Routes from "./Routes/index.svelte";

  export let url = "";
</script>

<style>
  .router {
    padding: 20px 30px;
  }
</style>

<Router {url}>
  <Navbar />
  <div class="router">
    <Routes />
  </div>
</Router>
