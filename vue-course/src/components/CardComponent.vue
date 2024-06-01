<script>
export default {
  name: "CardComponent",
  props: {
    title: String,
    text: String
  }
}
</script>

<template>
  <div v-if="title || text" class="card">
    <div class="card-body">
      <h4 v-if="title" class="card-title">{{ title }}</h4>
      <p v-if="text" class="card-text">{{ text }}</p>
    </div>
  </div>
</template>

<style scoped>

</style>