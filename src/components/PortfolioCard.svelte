<script>
  export let cardId;
  export let cardImgUrl;
  export let cardTitle;
  export let cardText;
  export let cardLinkDemoUrl;
  export let cardAlt;
  export let demoLinkClass;
  export let demoIcon;
</script>

<style>
  li {
    scroll-snap-align: center;
    height: 98vh;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  section {
    display: flex;
    flex-direction: row-reverse;
    justify-content: space-around;
    align-items: center;
    color: var(--text-secondary);
    background-color: #2b3942;
    border-radius: .5rem 0 0 .5rem;
    padding: 4rem 1rem;
  }

  figure {
    flex: 2;
  }

  img {
    width: 100%;
  }

  div {
    flex: 1;
    text-align: right;
  }

  h2 {
    color: #5e9159;
    text-shadow: 0 0 .75rem #5e9159;
    filter: grayscale(5%) opacity(0.9);
    font-size: 2rem;
  }

  p {
    font-size: 1.25rem;
  }

  @media (max-width: 600px) {
    section {
      flex-direction: column;
      /* justify-content: start; */
      padding: 0;
    }

    div {
      padding: 0 2rem;
    }
  }
</style>

<li id="{cardId}">
  <section>
    <figure>
      <img src="{cardImgUrl}" alt={cardAlt} />
    </figure>
    <div>
      <h2>{cardTitle}</h2>
      <p>
        {cardText}
      </p>
      <div>
        <a
          class="{demoLinkClass}"
          href="{cardLinkDemoUrl}"
          target="_blank"
          rel="noopener noreferrer"
        >
          <i class="{demoIcon}"></i>
        </a>
      </div>
    </div>
  </section>
</li>
