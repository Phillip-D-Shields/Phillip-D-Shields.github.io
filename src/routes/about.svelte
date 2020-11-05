<script>
  import { fade } from 'svelte/transition';
</script>

<style>
  section {
    width: 95%;
    height: 95%;
    margin: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    color: var(--text-primary);
  }

  figure {
	flex: 1;
	padding: .5rem;
  }
  img {
	  width: 100%;
	  height: auto;
  }
  div {
	flex: 2;
	padding: 1rem;
	display: flex;
	flex-direction: column;
	justify-content: space-around;
  }

  h1 {
    font-size: 3rem;
  }

  p {
    font-size: 1.25rem;
  }
  @media (max-width: 600px) {
    section {
      flex-direction: column;
    }
    div {
      justify-content: start;
      padding: 2rem;
    }
  }

</style>

<svelte:head>
  <title>About</title>
</svelte:head>

<section transition:fade>
  <figure>
    <img src="profile.png" alt="profile img" />
  </figure>
  <div>
    <h1>code panda</h1>
    <p>
      Hiya, I'm Phill. I am a former teacher and new front end guy. I also make
      high-tech water sports equipment for professional athletes, and a few
      olympians. I am currently studying Information Technology at Nelson
      Marlborough Institute of Technology in sunny Nelson, New Zealand.
    </p>
  </div>
</section>
