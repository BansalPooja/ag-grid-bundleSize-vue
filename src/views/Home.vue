<template>
  <div id="home">
    <img class="logo" src="../assets/logo.png" alt="logo" />
    <h1>👋Hello world🌎</h1>
     <ag-grid
    class="ag-theme-alpine"
    :column-defs="cols"
    :row-data="rowData"

  >
  </ag-grid>
  </div>
</template>
<script>
import { agGrid } from '@ag-grid-community/core';

export default {
  components: {
    Grid
  },
  data() {
      return {
        cols: ['Make', 'Model', 'Year', 'Color'],
        rows: [
          ['Ford', 'Fusion', '2011', 'Silver'],
          ['Chevrolet', 'Cruz', '2018', 'White']
        ]
      }
    }
}
</script>