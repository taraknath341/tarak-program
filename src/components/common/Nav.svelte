<script>
   import { IconHome, IconInfoCircle, IconVideo, IconUserCode, IconHeartHandshake } from "@tabler/icons-svelte-runes";
</script>

<header class="container">
   <nav>
      <ul>
         <li>
            <img src="https://taraknath341.codeberg.page/client_storage/logo.svg" alt="logo" />
         </li>
      </ul>
      <ul>
         <li><a href="/#/"><IconHome stroke={2} size={28} /></a></li>
         <li><a href="/#/about"><IconInfoCircle stroke={2} size={28} /></a></li>
         <li><a href="/#/video"><IconVideo stroke={2} size={28} /></a></li>
         <li><a href="https://taraknath341.github.io"><IconUserCode stroke={2} size={28} /></a></li>
         <li><a href="/#/supporters"><IconHeartHandshake stroke={2} size={28} /></a></li>
      </ul>
   </nav>
</header>

<style>
   header {
      position: sticky;
      top: 0;
      background: color-mix(in srgb, var(--pico-background-color) 70%, #00000000);
      backdrop-filter: blur(6px);
      z-index: 2;
   }
   img {
      box-shadow: 1px 1px 1pc var(--pico-primary);
      border-radius: 6px;
      height: 2pc;
   }
</style>
