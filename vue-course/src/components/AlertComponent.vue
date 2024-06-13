<script>
export default {
  name: 'AlertComponent',
  props: {
    text: {
      type: String,
      required: true
    },
    type: {
      type: String,
      required: true,
      validator: value => [
        'primary',
        'secondary',
        'success',
        'danger',
        'warning',
        'info',
        'light',
        'dark'
      ].includes(value)
    }
  },
  computed: {
    alertClasses() {
      return ['alert', `alert-${this.type}`, 'alert-dismissible', 'fade', 'show'];
    }
  }
};
</script>

<template>
  <div :class="alertClasses" role="alert">
    {{ text }}
  </div>

</template>

<style scoped>

</style>