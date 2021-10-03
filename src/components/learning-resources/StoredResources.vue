<template>
  <ul>
    <resource-item v-for='resource in resources'
                   :key='resource.id'
                   :resource='resource'></resource-item>
  </ul>
</template>

<script>
import ResourceItem from './ResourceItem';

export default {
  inject: ['resources'],
  components: {
    ResourceItem,
  },
}
</script>

<style>
ul {
  list-style: none;
  padding: 0;
  margin: auto;
  max-width: 40rem;
}
</style>
