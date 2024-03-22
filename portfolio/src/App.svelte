<script>
  import Home from "./components/Home.svelte";
  import MainServices from "./components/servicesComponents/MainServices.svelte";
  import { Router, Route } from "svelte-routing";
  import Services from "./components/Services.svelte";
</script>

<Router>
  <Route path="/" component={Home} />
  <Route path="services" component={Services} />
</Router>

<!-- <Home /> -->

<style>
  * {
    margin: 0;
    padding: 0;
    outline: 0;
    border: 0;
    appearance: 0;
    list-style: none;
    text-decoration: none;
    box-sizing: border-box;
  }
</style>
