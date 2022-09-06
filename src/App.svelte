<script>
  import logo from './assets/svelte.png'
  import pic from './assets/eric.png'
  import Counter from './lib/Counter.svelte'
  import Hero from './lib/Hero.svelte'
  import Nav from './lib/nav.svelte'
  import Tech from './lib/Tech.svelte';
  import Projects from './lib/Projects.svelte';
</script>

<main>
  <Nav />
  <Hero />
  <Projects />
  <Tech />
  
<!-- 
  <Counter /> -->

</main>

<style>


  :root {
    font-family: var(--font-sans)
  }

  *{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }






  @media (min-width: 480px) {
    h1 {
      max-width: none;
    }

    p {
      max-width: none;
    }
  }
</style>
