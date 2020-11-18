<script>
  import GitHub from './GitHub.svelte';
  import Nav from './Nav.svelte';
  import AppLogo from './AppLogo.svelte';
</script>

<style>
  .wrapper {
    display: grid;
    grid-template-columns: 150px 1fr 32px;
    align-items: center;
  }
</style>

<nav class="topbar">
  <div class="wrapper container">
    <AppLogo />
    <Nav />
    <GitHub />
  </div>
</nav>
