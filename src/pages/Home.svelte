<script>
   import Card from "../components/common/Card.svelte";
</script>

<main class="container">
   {#each program as { title, content, image, url }, i (i)}
      <Card {title} {content} {image} {url} />
   {/each}
</main>

<style>
   main {
      text-align: center;
   }
</style>
