<template>
  <div id="app">
    <div class="h-full bg-gray-300 p-3">
      <div class="flex w-full md:w-4/5 xl:w-2/5 mx-auto flex-col">
        <content-box class="mt-0 px-10 py-10 justify-between sm:flex-row">
          <div class="flex flex-col justify-center">
            <div class="text-5xl font-bold">김현우</div>
            <div>Backend Developer</div>
          </div>
          <div class="flex flex-col justify-between pt-5 md:pt-0">
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

        <content-box>
          <div class="mb-3 text-center text-lg md:text-2xl font-bold">
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

        <content-box>
          <div class="text-2xl font-bold mb-3">Education</div>
          <div class="flex flex-col md:flex-row flex-wrap">
            <div class="flex flex-row md:w-1/2 mb-3 items-center">
              <img
                src="@/assets/img/woowacourse-logo.jpg"
                alt="wooteco"
                class="w-12 h-12 mr-3"
              />
              <div class="flex flex-col mb-1">
                <a href="https://woowacourse.github.io/" target="_blank">
                  <div class="text-xl font-bold">우아한테크코스 2기</div>
                </a>
                <div class="text-gray-600">2020.02 ~ 2020.11</div>
                <div>백엔드 과정 수료</div>
              </div>
            </div>
            <div class="flex flex-row md:w-1/2 mb-3 items-center">
              <img
                src="@/assets/img/university-logo.jpg"
                alt="university"
                class="w-12 h-12 mr-3"
              />
              <div class="flex flex-col mb-1">
                <a href="https://mme.dongguk.edu/" target="_blank">
                  <div class="text-xl font-bold">동국대학교(서울)</div>
                </a>
                <div class="text-gray-600">2016.03 ~ (휴학)</div>
                <div>멀티미디어공학과 2학년 수료</div>
              </div>
            </div>
            <div class="flex flex-row md:w-1/2 mb-3 items-center">
              <img
                src="@/assets/img/highschool-logo.jpg"
                alt="highschool"
                class="w-12 h-12 mr-3"
              />
              <div class="flex flex-col mb-1">
                <a
                  href="https://www.dimigo.hs.kr/index.php?mid=class_wp"
                  target="_blank"
                >
                  <div class="text-xl font-bold">한국디지털미디어고등학교</div>
                </a>
                <div class="text-gray-600">2013.03 ~ 2016.02 (졸업)</div>
                <div>웹프로그래밍학과</div>
              </div>
            </div>
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
