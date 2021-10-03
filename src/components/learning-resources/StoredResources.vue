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
  components: {
    ResourceItem,
  },
 props: ['resources'],
}
</script>

<style>
ul {
  list-style: none;
  margin: 0;
  padding: 0;
  margin: auto;
  max-width: 40rem;
}
</style>
