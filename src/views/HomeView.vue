<script>
import QueensParkImage from '@/components/QueensParkImage.vue';
import tboLogo from '@/assets/tbo-logo.webp';
import { useRouter } from 'vue-router';


export default {
  components: {
    QueensParkImage
  },
  setup() {

    const router = useRouter();

    const goToPage = (page) => {
      router.push(page);
    }
    return {
      tboLogo,
      goToPage
    }
  }
}
</script>

<template>
  <div class="page-wrapper">
    <QueensParkImage />
    <main>
      <img :src="tboLogo" alt="Take Back Ontario Logo" class="large-image" />
      <h1 class="text-black my-10">IT’S YOUR PROVINCE. TAKE IT BACK.</h1>
      <p class="main-content">Ontario's managerial class has become unresponsive to the needs of everyday
        people because we stopped showing up. It's time for Ontarians to remember our strength and to remember the
        political power comes from our relationships. It's time for us to take back our institutions. It's time for
        Ontarians to Take Back Ontario.</p>
      <div class="buttons">
        <button @click="goToPage('about')" class="btn my-8">Learn&nbsp;More</button>
        <button @click="goToPage('events')" class="btn my-8" href="/events">Events</button>
        <button @click="goToPage('resources')" class="btn my-8" href="/resources">Resources</button>
        <a class="btn my-8" href="https://signup.takebackontario.ca">Join&nbsp;Us</a>
      </div>
    </main>
  </div>
</template>

<style scoped>
.page-wrapper {
  position: relative;
  display: block;
  width: 100%;
}
.buttons {
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
}
.large-image {
  width: 100%;
  margin: 0 auto;
  display: block;
}
.text-black {
  text-align: center;
  font-size: 3.5rem;
}
</style>