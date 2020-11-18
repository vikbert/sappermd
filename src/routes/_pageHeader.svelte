<script>
  export let pageTitle = '';
</script>

<svelte:head>
  <title>{pageTitle}</title>
</svelte:head>

<div class="hero is-primary">
  <div class="centered-xy my-2">
    <slot />
  </div>
</div>
