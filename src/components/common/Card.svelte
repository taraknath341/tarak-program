<script>
   import { IconExternalLink } from "@tabler/icons-svelte-runes";
   const { title, image, content, url } = $props();
</script>

<article>
   <h2>{title}</h2>
   {#if url}
      <a href={url}>
         <IconExternalLink stroke={2} size={35} />
      </a>
   {/if}

   {#if image}
      <img src={image} alt={title} width="80" />
   {/if}
   <p>{content}</p>
</article>

<style>
   h2 {
      color: var(--pico-primary);
      text-shadow: 1px 1px 2pc var(--pico-primary);
   }

   article {
      position: relative;
      text-align: start;
      border-radius: 1pc 2pc;
      box-shadow: 3px 3px 1px var(--pico-primary);
      margin: 0.5pc;
      width: 47%;
      display: inline-block;
      &:hover {
         transform: translate(3px, 3px);
         box-shadow: 0px 0px 0px var(--pico-primary);
      }

      img {
         box-shadow: 1px 1px 1pc var(--pico-primary);
         float: right;
         margin: 0.2pc;
         border-radius: 1pc;
      }

      a {
         position: absolute;
         top: 0.7pc;
         right: 1pc;
      }
   }

   /* Mobile Design */
   @media (max-width: 768px) {
      article {
         width: 98%;
      }
   }
</style>
