<script>
  import Cell from './Cell.svelte';

  const maxCells = 9;
</script>

<div class="board" role="grid">
  <div class="row" role="row">
      <Cell />
      <Cell />
      <Cell />
  </div>
  <div class="row" role="row">
      <Cell />
      <Cell />
      <Cell />
  </div>
  <div class="row" role="row">
      <Cell />
      <Cell />
      <Cell />
  </div>
</div>

<style>
  .board {
    display: flex;
    flex-direction: column;
    border: 4px solid var(--darkgray);
  }
  .board > * {
    border: none;
  }
  .board > * + * {
    border-top: 4px solid var(--darkgray);
  }
  .row {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
  }
  :global(.row > * ) {
    border: none;
  }
  .row > :global(* + *) {
    border-left: 4px solid var(--darkgray);
  }
</style>