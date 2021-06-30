<script>
 export let row;
 export let cellNumber;
</script>

<button class="cell" role="gridcell">

</button>

<style>
  .cell {
    aspect-ratio: 1 / 1;
    background-color: var(--blackish);
    transition: all 300ms ease-in-out;
    outline-offset: -4px;
  }

  .cell:hover {
    background-color: var(--lightblackish);
  }

  .cell:active, .cell:focus {
    outline: 4px solid var(--blue);
    background-color: var(--lightlightblackish);
  }
</style>