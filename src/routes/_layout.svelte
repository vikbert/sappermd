<script>
  import Topbar from '../components/topbar/index.svelte';
  import Footer from '../components/footer/index.svelte';
</script>

<Topbar />

<main class="main container">
  <slot />
</main>

<Footer />
