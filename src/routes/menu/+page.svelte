<script>
  const menus = [
    {
      title: "Menu dei vini",
      img: "wine",
      desc: "",
      url: "https://dnnr.it/view/pescou-vini",
    },
  ];
</script>

<svelte:head>
  <title>Menu | Trattoria U Pescou</title>
  <meta
    name="description"
    content="Scopri i menu della Trattoria U Pescou a Lavagna: piatti di pesce fresco, cucina tipica ligure e la nostra carta dei vini."
  />
  <link rel="canonical" href="https://upescou.it/menu" />

  <meta property="og:title" content="Menu | Trattoria U Pescou" />
  <meta
    property="og:description"
    content="Scopri i menu della Trattoria U Pescou a Lavagna: piatti di pesce fresco, cucina tipica ligure e la nostra carta dei vini."
  />
  <meta property="og:url" content="https://upescou.it/menu" />
  <meta property="og:image" content="https://upescou.it/img/23.webp" />

  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="Menu | Trattoria U Pescou" />
  <meta
    name="twitter:description"
    content="Scopri i menu della Trattoria U Pescou a Lavagna: piatti di pesce fresco, cucina tipica ligure e la nostra carta dei vini."
  />
  <meta name="twitter:image" content="https://upescou.it/img/23.webp" />
</svelte:head>

<h1 class="sr-only">Menu della Trattoria U Pescou</h1>

<div
  class="min-h-64 min-w-screen bg-slate-300 mb-8 bg-cover"
  style="background-image: url(/img/23.webp);"
></div>

<div
  class="min-h-screen flex flex-wrap justify-center align-center gap-3 p-11 mx-auto max-w-screen-lg"
>
  {#each menus as m}
    <a class="card bg-base-100 w-96 shadow-xl h-96" href={m.url}>
      <figure>
        <img src="/img/{m.img}.webp" alt={m.title} />
      </figure>
      <div class="card-body">
        <h2 class="card-title">{m.title}</h2>
        <p>{m.desc}</p>
      </div>
    </a>
  {/each}
</div>
<div id="servizi"></div>
<div id="contatti"></div>
