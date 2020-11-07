<template>
  <div id="app">
    <div class="h-screen bg-green-100">
      <div class="flex w-3/4 xl:w-1/2 mx-auto pt-5 flex-col">
        <div class="info flex w-full p-10 bg-white justify-between">
          <div>
            <div class="text-5xl font-bold">김현우</div>
            <div>Backend Developer</div>
          </div>
          <div>
            <div class="py-3">
              <a href="https://github.com/hwookim" target="_blank"> hwookim </a>
            </div>
            <div class="py-3">
              <a href="mailto:gusdn9754@gmail.com" target="_blank">
                gusdn9754@gmail.com
              </a>
            </div>
          </div>
        </div>

        <div class="info w-full mx-auto my-2 py-2 bg-white">
          <div class="calendar w-11/12"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import 'github-calendar/dist/github-calendar-responsive.css';
import GitHubCalendar from 'github-calendar';

export default {
  name: 'App',
  mounted() {
    GitHubCalendar('.calendar', 'hwookim', {
      responsive: true,
      cache: 3600,
      global_stats: false,
    });
  },
};
</script>
