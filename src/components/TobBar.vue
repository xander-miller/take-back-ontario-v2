<template>
  <div class="top-bar">
      <img @click="backToHome" :src="tboLogo" alt="Take Back Ontario Logo" class="subpage-logo" />
  </div>
</template>

<script>
import tboLogo from '@/assets/tbo-logo.webp'
import { useRouter } from 'vue-router'

export default {

  setup() {
    const router = useRouter();
    const backToHome = () => {
      router.push('/')
    }
    return {
      tboLogo,
      backToHome
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
  cursor: pointer;
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