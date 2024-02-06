<script>
export default {
  name: 'Header',
};
</script>

<template>
  <header class="mb-10 p-6 text-center text-white bg-blue-800">
    <div class="mb-3 text-3xl md:text-5xl font-bold">
      <i class="fa fa-viruses"></i> Covid-19 Tracker
    </div>
    <p>
      API by
      <a class="text-blue-300" href="https://covid19-brazil-api.now.sh/api/report/v1/brazil" target="_blank"
        >https://covid19-brazil-api.now.sh/api/report/v1/brazil</a
      >
    </p>
  </header>
</template>
