<script>
  import { fly } from "svelte/transition";
</script>

<style>
    section {
        width: 100%;
        height: 100%;
        overflow: hidden;
    }
  ul {
    scroll-snap-type: y mandatory;
    overflow-y: scroll;
    height: 100%;
    width: 100%;
  }
 
</style>

<section transition:fly="{{ y: 400, duration: 1000 }}">
  <ul>
    <slot></slot>
  </ul>
</section>