<script>
export default {
  name: 'BtnGroup',
  data() {
    return {
      buttons: [
        { label: 'Left', type: 'secondary', active: false },
        { label: 'Right', type: 'secondary', active: false }
      ]
    };
  },
  methods: {
    activateButton(index) {
      this.buttons.forEach((button, i) => {
        this.$set(button, 'active', (i === index));
      });
    }
  }
};
</script>

<template>
  <div class="btn-group" role="group">
    <button
        v-for="(button, index) in buttons"
        :key="index"
        type="button"
        class="btn"
        :class="{ 'btn-secondary': button.type === 'secondary' && !button.active, 'btn-primary': button.type === 'primary' || button.active, active: button.active }"
        @click="activateButton(index)"
    >
      {{ button.label }}
    </button>
  </div>
</template>

<style scoped>
.btn {
  margin-right: 10px;
}

.active {
  background-color: #007bff;
  color: white;
}
</style>