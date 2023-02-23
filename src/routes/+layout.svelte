<script>
  import NavBar from "$lib/NavBar.svelte";
  import "../app.css";

  import { appWindow } from "@tauri-apps/api/window";
  document
    .getElementById("titlebar-minimize")
    ?.addEventListener("click", () => appWindow.minimize());
  document
    .getElementById("titlebar-maximize")
    ?.addEventListener("click", () => appWindow.toggleMaximize());
  document
    .getElementById("titlebar-close")
    ?.addEventListener("click", () => appWindow.close());
</script>

<main class="container">
  <NavBar />
  <slot />
</main>
