<script lang="typescript">
  export let title: string = "Dynameek";
  import RecentBuilds from "../components/RecentBuilds.svelte";
</script>

<svelte:head>
  <title>{title}</title>
</svelte:head>

<article class="container clearfix">
  <h1>{title}</h1>
  <h2>A Software Development &amp; Consultancy Services Company.</h2>
  <h3>What we do...</h3>
  <p>
    At {title}, we like to get things 'done'.&nbsp; We don’t aim for perfection,
    we take a artisan's approach to continually improving results for you and
    delivering better technology outcomes for your business.
  </p>
  <ul class="what-we-do">
    <li>Application & API Development</li>
    <li>Mobile Development</li>
    <li>UX</li>
    <li>Cloud Migration</li>
  </ul>

  <h3>Who we've worked with...</h3>
  <RecentBuilds />
  <div class="email">
    <p>
      <a href="mailto:hello@dynameek.co.uk">hello@dynameek.co.uk</a>
    </p>
  </div>
</article>
