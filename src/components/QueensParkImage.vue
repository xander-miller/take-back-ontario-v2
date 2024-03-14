<script>
import qpBackground from '@/assets/queens-park-background.jpg'

export default {
  setup() {
    return {
      qpBackground
    }
  }
}
</script>


<template>
  <img :src="qpBackground" alt="Queen's Park Background" class="qp-background" />
</template>

<style scoped>
.qp-background {
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  height: auto;
  z-index: -2;
}
</style>