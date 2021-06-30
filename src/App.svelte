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
    display: flex;
    justify-content: center;
    align-items: center;
    width: clamp(320px, 60vw, 680px);
    margin-inline: auto;
  }
  .content {
    width: 100%;
    margin-block: 2rem;
  }
</style>