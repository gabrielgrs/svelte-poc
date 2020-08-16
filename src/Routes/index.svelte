<script>
  import { Router, Route } from "svelte-routing";
  import Home from "../containers/Home.svelte";
  import About from "../containers/About.svelte";
  import Demo from "../containers/Demo.svelte";
</script>

<Route path="demo" component={Demo} />
<Route path="about" component={About} />
<Route path="/" component={Home} />
