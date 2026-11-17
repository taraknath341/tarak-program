<script>
   // components
   import Nav from "./components/common/Nav.svelte";
   import Bottom from "./components/common/Bottom.svelte";
   import Router from "svelte-spa-router";
   // pages
   import Home from "./pages/Home.svelte";
   import About from "./pages/About.svelte";
   import Video from "./pages/Video.svelte";
   import Supporters from "./pages/Supporters.svelte";
   import NotFound from "./pages/NotFound.svelte";
</script>

<Nav />

<Router
   routes={{
      "/": Home,
      "/about": About,
      "/video": Video,
      "/supporters": Supporters,
      "*": NotFound,
   }}
/>

<Bottom />
