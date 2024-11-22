<template>
  <div class="home">
    <YappoMeter/>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import YappoMeter from '@/components/YappoMeter.vue';

@Options({
  components: {
    YappoMeter,
  },
})
export default class HomeView extends Vue {}
</script>

<style scoped>
  .home {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
</style>