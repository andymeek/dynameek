<script>
  import Header from "../components/Header.svelte";
  import Footer from "../components/Footer.svelte";
</script>

<style lang="scss" global>
  @import "../styles/main.scss";
</style>

<Header />

<main>
  <slot />
</main>

<Footer />
