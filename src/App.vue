<template>
  <div id="app">
    <div class="h-screen bg-gray-300">
      <div class="flex w-full md:w-4/5 xl:w-2/5 mx-auto pt-5 flex-col">
        <content-box class="p-10 justify-between sm:flex-row">
          <div>
            <div class="text-5xl font-bold">김현우</div>
            <div>Backend Developer</div>
          </div>
          <div class="flex flex-col justify-between">
            <div class="flex items-center">
              <i class="mdi mdi-cellphone text-2xl mr-2" />
              010-3020-9754
            </div>
            <div>
              <a
                href="mailto:gusdn9754@gmail.com"
                target="_blank"
                class="flex items-center"
              >
                <i class="mdi mdi-email text-2xl mr-2" />
                gusdn9754@gmail.com
              </a>
            </div>
            <div>
              <a
                href="https://github.com/hwookim"
                target="_blank"
                class="flex items-center"
              >
                <i class="mdi mdi-github text-2xl mr-2" />
                github.com/hwookim
              </a>
            </div>
          </div>
        </content-box>

        <content-box class="py-3 justify-center">
          <div class="mb-3 text-center text-2xl font-bold">
            🐢 꾸준히 한걸음씩 나아가는 중입니다 🐢
          </div>
          <div>
            <a href="https://github.com/hwookim" target="_blank">
              <img
                src="http://ghchart.rshah.org/hwookim"
                alt="hwookim's Github chart"
                class="w-full"
              />
            </a>
          </div>
        </content-box>
      </div>
    </div>
  </div>
</template>

<script>
import ContentBox from '@/component/ContentBox.vue';

export default {
  name: 'App',
  components: { ContentBox },
};
</script>
