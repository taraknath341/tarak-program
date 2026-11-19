<script>
   import Card from "../components/common/Card.svelte";
</script>

<main class="container">
   {#each about as { title, content, image }, i (i)}
      <Card {title} {content} {image} />
   {/each}
</main>

<style>
   main {
      text-align: center;
   }
</style>
