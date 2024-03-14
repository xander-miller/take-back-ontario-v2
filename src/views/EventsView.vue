<script setup>
import TobBar from '@/components/TobBar.vue';
import QueensParkImage from '@/components/QueensParkImage.vue';

</script>

<template>
  <div class="page-wrapper">
    <TobBar />
    <QueensParkImage />
    <main>
      <h1>Upcoming Events</h1>
      <div class="main-content">
        <h2>Weekly Zoom Meetings</h2>
        <p>
          Weekly Zoom meetings are held every Wednesday at 7:00pm. These meetings are hosted by TBO founder Xander
          Miller or a guest host.
          These meetings focus on growing the movement, with guidance from David Parker (from Take Back Alberta) and his
          longtime associates.
        </p>
        <p>
          Sign up at the "Join Us" link below to receive the Zoom link for these meetings.
        </p>
        <a class="btn my-8" href="https://signup.takebackontario.ca">Join Us</a>
        <h2>In-person Meetings</h2>

        <p>
          Stay tuned! As we collect a membership list with postal codes, we will be able to send introduction emails to
          members who are geographically close to one another.
          Members can then organize in-person meetings in their area.
        </p>
      </div>
    </main>
  </div>
</template>
