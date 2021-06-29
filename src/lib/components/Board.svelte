<script>

</script>

<div class="board" role="grid">
  <div class="row" role="row">
      <button class="cell" role="gridcell">Cell</button>
      <button class="cell" role="gridcell">Cell</button>
      <button class="cell" role="gridcell">Cell</button>
  </div>
  <div class="row" role="row">
      <button class="cell" role="gridcell">Cell</button>
      <button class="cell" role="gridcell">Cell</button>
      <button class="cell" role="gridcell">Cell</button>
  </div>
  <div class="row" role="row">
      <button class="cell" role="gridcell">Cell</button>
      <button class="cell" role="gridcell">Cell</button>
      <button class="cell" role="gridcell">Cell</button>
  </div>
</div>

<style>
  .board {
    display: grid;
    grid-template-rows: repeat(3, 1fr);
    min-height: 100%;
    border: 1px solid var(--blackish);
  }
  .row {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    justify-self: stretch;
  }
  .cell {
    aspect-ratio: 1 / 1;
    border: none;
  }
</style>