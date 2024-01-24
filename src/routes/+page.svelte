<script>
  import About from '../components/About.svelte';
  import Specialties from '../components/Specialties.svelte';
  import Media from '../components/Media.svelte';
  import Contact from '../components/Contact.svelte';
  import Hero from '../components/Hero.svelte';
</script>

<Hero />
<main>
  <Specialties />
  <About />
  <Media />
  <Contact />
</main>

<style>
  main {
    display: flex;
    flex-direction: column;
    min-width: fit-content;
    max-width: 1100px;
    justify-content: flex-start;
    margin: 0 auto;
  }
</style>
