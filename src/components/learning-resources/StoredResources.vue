<template>
  <ul>
    <learning-resource
      v-for="res in resources"
      :key="res.id"
      v-bind="res"
    ></learning-resource>
  </ul>
</template>

<script>
import LearningResource from './LearningResource.vue';

export default {
  components: {
    LearningResource,
  },
  inject: ['resources'],
};
</script>

<style scoped>
ul {
  list-style: none;
  margin: auto;
  max-width: 40rem;
}
</style>
