<script>
export default {
  name: "ListGroup"
}
</script>

<template>
  <ul class="list-group">
    <slot></slot>
  </ul>
</template>

<style scoped>
.list-group {
  margin-bottom: 20px;
}

.list-group-item {
  background-color: #f0f0f0;
  border: 1px solid #ccc;
  padding: 10px;
  margin-bottom: 5px;
}

</style>