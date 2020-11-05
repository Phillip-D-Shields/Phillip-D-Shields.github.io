<script>
  export let segment;
</script>

<style>
  nav {
    background-color: #2B3942;
    position: fixed;

  }

  ul {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    flex-direction: column;
    height: 100%;
  }

  li {
    width: 100%;
  }

  .logo {
    margin-bottom: 1rem;
    width: 100%;
    padding: 1rem;
    color: #c26838;
  }

  .logo i {
    transform: rotate(0deg);
    transition: var(--transition-speed);
    filter: grayscale(10%) opacity(0.8);
  }

  nav:hover .logo i {
    transform: rotate(-180deg);
    color: #c26838;
    text-shadow: 0 0 .75rem #c26838;
    filter: grayscale(0%) opacity(1);
  }

  a {
    width: 100%;
    display: flex;
    flex-direction: row-reverse;
    justify-content: start;
    align-items: center;
    height: 5rem;
    color: var(--text-primary);
    text-decoration: none;
    filter: grayscale(100%) opacity(0.7);
    transition: 200ms;
    
  }

  a:hover {
    filter: grayscale(0%) opacity(1);
    color: #a99245;
    text-shadow: 0 0 .75rem #a99245;
  }

  a i {
    width: 2rem;
    min-width: 2rem;
    margin: 0 1.5rem;
    display: block;
  }

  .selected {
    color: #5e9159;
    text-shadow: 0 0 .75rem #5e9159;
    filter: grayscale(5%) opacity(0.9);
  }

  /* Small screens */
  @media (max-width: 600px) {
    nav {
      bottom: 0;
      width: 100vw;
      height: 5rem;
    }

    .logo {
      display: none;
    }

    ul {
      flex-direction: row;
    }

    a {
      justify-content: center;
    }
  }
  /* Large screens */
  @media (min-width: 600px) {
    nav {
      top: 0;
      width: 5rem;
      height: 100vh;
      z-index: 10;
    }
  }
</style>

<nav>
  <ul>
    <li class="logo">
      <i class="fab fa-galactic-republic fa-3x"></i>
    </li>
    <li>
      <a class:selected={segment === undefined} aria-current='{segment === undefined ? "page" : undefined}' href=".">
        
        <i class="fas fa-globe fa-2x"></i>
      </a>
    </li>
    <li>
      <a class:selected={segment === "about"} aria-current='{segment === "about" ? "page" : undefined}' href="about"
        > <i class="fas fa-user-astronaut fa-2x"></i
      ></a>
    </li>
    <li>
      <a class:selected={segment === "portfolio"} aria-current='{segment === "portfolio" ? "page" : undefined}' href="portfolio"
      > <i class="fas fa-atom fa-2x"></i
    ></a>
    </li>
    <li><a href="#"><i class="fab fa-linkedin fa-2x"></i></a></li>
    <li><a href="#"><i class="fab fa-github-square fa-2x"></i></a></li>
  </ul>
</nav>
