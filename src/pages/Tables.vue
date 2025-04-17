<template>
  <q-page class="q-pa-sm">
    <TablesBasic />

    <TableActions class="q-mt-lg" />
    <TableDarkMode class="q-mt-lg" />
    <TableProgress class="q-mt-lg" />
    <TableCustomGrid class="q-mt-lg" />
  </q-page>
</template>

<script setup>
import { defineAsyncComponent } from "vue";

const TableProgress = defineAsyncComponent(() =>
  import("components/tables/TableProgress.vue")
);
const TableCustomGrid = defineAsyncComponent(() =>
  import("components/tables/TableCustomGrid.vue")
);
const TableDarkMode = defineAsyncComponent(() =>
  import("components/tables/TableDarkMode.vue")
);
const TableActions = defineAsyncComponent(() =>
  import("components/tables/TableActions.vue")
);
const TablesBasic = defineAsyncComponent(() =>
  import("components/tables/TableBasic.vue")
);
</script>

<style>
/* Optional custom styles */
</style>
