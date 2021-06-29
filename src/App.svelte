<script>
  import Header from './lib/components/Header.svelte';
  import Footer from './lib/components/Footer.svelte';
  import Board from './lib/components/Board.svelte';
</script>

<Header />
<main>
  <div class="content">
    <Board />
  </div>
</main>
<Footer />
<style>
  main {
    position: relative;
  }
  .content {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    display: grid;
  }
</style>