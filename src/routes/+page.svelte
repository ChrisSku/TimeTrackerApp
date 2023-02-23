<script>
  import Greet from "$lib/Greet.svelte";
</script>

<h1>Welcome to Timetracker!</h1>

<div class="row">
  <a href="/about" target="_self">
    <img src="/svelte.svg" class="logo svelte" alt="Svelte Logo" />
  </a>
</div>

<p>Click on the Tauri, Vite, and Svelte logos to learn more.</p>

<div class="row">
  <Greet />
</div>

<style>
  .logo.svelte:hover {
    filter: drop-shadow(0 0 2em #ff3e00);
  }
</style>
