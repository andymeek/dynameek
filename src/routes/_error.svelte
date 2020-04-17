<script>
  export let status;
  export let error;

  const dev = process.env.NODE_ENV === "development";
</script>

<svelte:head>
  <title>{status}</title>
</svelte:head>

<article class="container clearfix">
  <h1>Dynameek</h1>
  <h2>Error {error.message}</h2>
  <p>The page you're looking for doesn't exist.</p>
  <p>
    Please
    <a href="/">click here</a>
    to go home.
  </p>

  {#if dev && error.stack}
    <pre>{error.stack}</pre>
  {/if}
</article>
