<script>
export default {
  name: 'ProgressComponent',
  props: {
    percentage: {
      type: Number,
      required: true,
      validator: function(value) {
        return value >= 0 && value <= 100;
      }
    }
  }
};
</script>

<template>
  <div class="progress-bar" role="progressbar" :aria-valuenow="percentage" aria-valuemin="0" aria-valuemax="100">
    <div class="progress" :style="{ width: percentage + '%' }"></div>
  </div>
</template>

<style scoped>
.progress-bar {
  width: 100%;
  height: 1.5rem;
  background-color: #e0e0e0;
  border-radius: 0.5rem;
  overflow: hidden;
}

.progress {
  height: 100%;
  background-color: #4caf50;
  transition: width 0.3s ease;
}

</style>