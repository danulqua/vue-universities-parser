<template>
  <div class="spinner"></div>
</template>

<script>
export default {
  name: 'SpinnerBlock'
};
</script>

<style lang="scss" scoped>
@import '@/scss/variables';

.spinner {
  margin: 0 auto;
  width: 100px;
  height: 100px;
  border: 10px solid lighten($main-color, 35%);
  border-top-color: $main-color;
  border-radius: 50%;
  animation: spin linear infinite 1s;
}

@keyframes spin {
  0% {
    transform: rotate(0);
  }
  100% {
    transform: rotate(360deg);
  }
}
</style>
