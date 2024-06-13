<script>
export default {
  name: "DefinitionsList",
  props: {
    data: {
      type: Array,
      required: true,
    },
  },
};
</script>

<template>
  <dl>
    <div v-for="item in data" :key="item.id">
      <dt>{{ item.dt }}</dt>
      <dd>{{ item.dd }}</dd>
    </div>
  </dl>
</template>
<style scoped>

</style>