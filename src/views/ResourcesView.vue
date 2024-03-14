<script setup>
import QueensParkImage from '@/components/QueensParkImage.vue';
import TobBar from '@/components/TobBar.vue';

</script>

<template>
  <div class="page-wrapper">
    <TobBar />
    <QueensParkImage />
    <main>
      <h1>Resources</h1>
      <div class="main-content">
        <div>
          <ul>
            <li><a
                href="https://www.elections.on.ca/content/dam/NGW/sitecontent/2017/preo/Provincial%20Electoral%20Districts%20Map.zip"
                target="_blank">Provincial Electoral Districts Map</a></li>
            <li><a href="https://finances.elections.on.ca/en/contributions?fromYear=2014&toYear=2024"
                target="_blank">Ontario Political Contributions List</a></li>
          </ul>
        </div>
      </div>
    </main>
  </div>
</template>
