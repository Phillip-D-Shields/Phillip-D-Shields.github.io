<script>
  import PortfolioCard from "./../components/PortfolioCard.svelte";
  import PortfolioSlider from "./../components/PortfolioSlider.svelte";

  const cards = [
    {
      id: 0,
      cardImgUrl: "intC19.png",
      cardAlt: "next tachyons covid app",
      cardTitle: "International C19 Data Tracker",
      cardText: "Personal project using NextJs, Tachyons, and ChartJs",
      demoLinkClass: "card-link",
      cardLinkDemoUrl: "https://int-c19.vercel.app/",
      demoIcon: "far fa-eye fa-2x",
    },
    {
      id: 1,
      cardImgUrl: "bimbos.jpg",
      cardAlt: "bimbos pizza screenshot",
      cardTitle: "Bimbos Pizza",
      cardText: "Personal project for a hometown favorite.",
      demoLinkClass: "card-link",
      cardLinkDemoUrl: "https://phillip-d-shields.github.io/bimbos-pizza",
      demoIcon: "far fa-eye fa-2x",
    },
    {
      id: 2,
      cardImgUrl: "dcg.png",
      cardAlt: "dc genesis screenshot",
      cardTitle: "DC Genesis",
      cardText:
        "Landing page for a good friends business. The original DecentraCorp facility.",
      demoLinkClass: "card-link",
      cardLinkDemoUrl: "https://decentracorp.github.io/genesis",
      demoIcon: "far fa-eye fa-2x",
    },
    {
      id: 3,
      cardImgUrl: "nsw.jpg",
      cardAlt: "nari sawi screenshot",
      cardTitle: "Nari Sewa Kendra",
      cardText:
        " UN volunteer non-profit upgrade submission. Final round selection, but ultimately was not selected.",
      demoLinkClass: "card-link",
      cardLinkDemoUrl: "https://phillip-d-shields.github.io/Nari-Sewa-Kendra/",
      demoIcon: "far fa-eye fa-2x",
    },
    {
      id: 4,
      cardImgUrl: "jump.jpg",
      cardAlt: "jumpstart screenshot",
      cardTitle: "Jumpstart",
      cardText: "CodeCademy intensive project.",
      demoLinkClass: "card-link",
      cardLinkDemoUrl: "https://phillip-d-shields.github.io/jumpstart",
      demoIcon: "far fa-eye fa-2x",
    },
    {
      id: 5,
      cardImgUrl: "dc-react.png",
      cardAlt: "decentracorp react screenshot",
      cardTitle: "DecentraCorp react upgrade",
      cardText:
        "Prototype for a DecentraCorp upgrade. Utilizing reusable components.",
      demoLinkClass: "card-link",
      cardLinkDemoUrl: "https://elastic-almeida-ef8aa4.netlify.com/",
      demoIcon: "far fa-eye fa-2x",
    },
    {
      id: 6,
      cardImgUrl: "usMiC19.png",
      cardAlt: "svelte tachyons covid app",
      cardTitle: "US and MI C19 Data Tracker",
      cardText: "Personal project using Svelte, Tachyons, and ChartJs",
      demoLinkClass: "card-link",
      cardLinkDemoUrl: "https://clever-austin-0ad17d.netlify.app/",
      demoIcon: "far fa-eye fa-2x",
    },
  ];
</script>


  <PortfolioSlider>
    {#each cards as card}
      <PortfolioCard {...card} />
    {/each}
  </PortfolioSlider>

