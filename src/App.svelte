<script>
  import logo from './assets/svelte.png'
  import pic from './assets/eric.png'
  import Counter from './lib/Counter.svelte'
  import Hero from './lib/Hero.svelte'
</script>

<main>
  <Hero />
<!-- 
  <Counter /> -->

</main>

<style>


  :root {
    font-family: var(--font-sans)
  }

  *{
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
