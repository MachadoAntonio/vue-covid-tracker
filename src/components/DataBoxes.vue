<script>
export default {
  name: 'DataBoxes',
  props: ['stats'],
  methods: {
    numberWithCommas(num) {
      return num.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ',');
    },
  },
};
</script>

<template>
  <div class="grid md:grid-cols-2 gap-4">
    <!-- Box1 -->
    <div class="shadow-md bg-blue-100 p-10 text-center rounded">
      <h3 class="text-3xl text-blue-900 font-bold mb-4">Casos</h3>
      <div class="text-2xl mb-4">
        <span class="font-bold">New: </span>
        {{ numberWithCommas(stats.NewConfirmed) }}
      </div>
      <div class="text-2xl mb-4">
        <span class="font-bold">Total: </span>
        {{ numberWithCommas(stats.TotalConfirmed) }}
      </div>
    </div>

    <!-- Box2 -->
    <div class="shadow-md bg-blue-200 p-10 text-center rounded">
      <h3 class="text-3xl text-blue-900 font-bold mb-4">Mortes</h3>
      <div class="text-2xl mb-4">
        <span class="font-bold">New: </span>
        {{ numberWithCommas(stats.NewDeaths) }}
      </div>
      <div class="text-2xl mb-4">
        <span class="font-bold">Total: </span>
        {{ numberWithCommas(stats.TotalDeaths) }}
      </div>
    </div>
  </div>
</template>
