<template>
  <div class="top-bar">
    <a href="/">
      <img :src="tboLogo" alt="Take Back Ontario Logo" class="subpage-logo" />
    </a>
  </div>
</template>

<script>
import tboLogo from '@/assets/tbo-logo.webp'

export default {
  setup() {
    return {
      tboLogo
    }
  }
}
</script>


<style scoped>
.subpage-logo {
  position: relative;
  height: 100%;
  width: auto;
  max-width: 200px;
  padding: 1em;
}

.top-bar {
  display: flex;
  justify-content: center;
  position: relative;
  top: 0;
  left: 0;
  width: 100%;
  height: 80px;
  z-index: 1;
  border-bottom: 1px solid #d0d0d0;
}
</style>