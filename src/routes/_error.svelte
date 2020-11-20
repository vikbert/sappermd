<script>
  export let status;
  export let error;

  const dev = process.env.NODE_ENV === 'development';
</script>

<svelte:head>
  <title>{status}</title>
</svelte:head>

<div class="hero is-info">
  <div class="container centered-xy">
    <h2 class="bold">ERROR</h2>
  </div>
</div>

<div class="my-2">
  <h4>{status}</h4>

  <p>{error.message}</p>

  {#if dev && error.stack}
    <pre>{error.stack}</pre>
  {/if}
</div>
