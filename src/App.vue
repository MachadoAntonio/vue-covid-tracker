<script>
import Header from '@/components/Header';

export default {
  name: 'App',
  components: {
    Header,
  },
};
</script>

<template>
  <Header />
  <div class="container">
    <router-view />
  </div>
</template>
