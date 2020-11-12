<template>
  <div id="app">
    <div class="h-full bg-gray-300 p-3">
      <div class="flex w-full md:w-4/5 xl:w-1/2 mx-auto flex-col">
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

        <content-box title="What I can">
          <skill-box type="BackEnd">
            Java, JUnit5, Mockito, Spring Boot, Spring Data JPA
          </skill-box>
          <skill-box type="FrontEnd"> JavaScript(ES6), Vue2 </skill-box>
          <skill-box type="Infra"> AWS EC2, Jenkins, Nginx, Linux </skill-box>
        </content-box>

        <content-box title="About Me">
          <div>
            <toggle-box>
              <template v-slot:title>
                테스트 작성을 당연하게 생각합니다.
              </template>
              <template v-slot:content>
                <li>
                  우아한테크코스에서 처음으로 웹 개발을 배우면서 항상 테스트가
                  있는 코드만을 접해왔습니다.
                </li>
                <li>
                  Junit5를 통해 TDD 사이클의 개발을 자연스럽게 익혀왔습니다.
                </li>
                <li>
                  테스트가 없는 코드에 불안해하고 테스트를 통해 안정성을
                  보장하고 싶어합니다.
                </li>
              </template>
            </toggle-box>

            <toggle-box>
              <template v-slot:title>
                다양한 방법으로 의견을 공유하고 설득하고 설득당하는 걸 즐깁니다.
              </template>
              <template v-slot:content>
                <li>코드리뷰를 통해 더 나은 코드를 추구합니다.</li>
                <li>
                  우아한 테크코스에서 운영하는 기술 블로그를 통해 배운 지식을
                  공유합니다.
                </li>
              </template>
            </toggle-box>

            <toggle-box>
              <template v-slot:title>
                Spring framework를 통해 웹 서버를 구축할 수 있습니다.
              </template>
              <template v-slot:content>
                <li>
                  우아한 테크코스에서 Spring Data JDBC와 JPA를 이용한 RestfulAPI
                  Application 구현 방법에 대해 학습했습니다.
                </li>
              </template>
            </toggle-box>

            <toggle-box>
              <template v-slot:title>
                Vue.js로 간단한 반응형 웹 페이지를 구현할 수 있습니다.
              </template>
              <template v-slot:content>
                <li>현재 보고 계신 페이지를 템플릿 없이 직접 구현했습니다.</li>
              </template>
            </toggle-box>

            <toggle-box>
              <template v-slot:title>
                하나의 서비스에 필요한 최소한의 인프라 환경을 구축할 수
                있습니다.
              </template>
              <template v-slot:content>
                <li>
                  nginx를 통해 정적 웹 페이지 서버를 구축하고 원하는 환경을
                  설정할 수 있습니다.
                </li>
                <li>
                  Jenkins의 Publish over SSH와 Shell Script를 통해 Blue-Green
                  방식의 무중단 배포 환경을 구축했습니다.
                </li>
              </template>
            </toggle-box>

            <toggle-box>
              <template v-slot:title>
                더 나은 방법, 더 나은 가치를 향해 끊임없이 고민합니다.
              </template>
              <template v-slot:content>
                <li>
                  개발 도중 막히는 부분이 생기면 밤을 새서라도 해결하고
                  싶어합니다.
                </li>
                <li>
                  최근 1일 1커밋 운동을 시작했습니다.<br />
                  이를 통해 꾸준히 성장하는 자세를 잃지 않으려고 노력 중입니다.
                  <a href="https://github.com/hwookim" target="_blank">
                    <img
                      src="http://ghchart.rshah.org/hwookim"
                      alt="hwookim's Github chart"
                      class="my-3"
                    />
                  </a>
                </li>
              </template>
            </toggle-box>
          </div>
        </content-box>

        <content-box title="Education">
          <div class="flex flex-col md:flex-row flex-wrap">
            <education-item
              src="https://woowacourse.github.io/"
              name="우아한테크코스 2기"
              period="2020.02 ~ 2020.11"
              description="백엔드 과정 수료"
            >
              <img src="@/assets/img/woowacourse-logo.jpg" alt="wooteco" />
            </education-item>
            <education-item
              src="https://mme.dongguk.edu/"
              name="동국대학교(서울)"
              period="2016.03 ~ (휴학)"
              description="멀티미디어공학과 2학년 수료"
            >
              <img src="@/assets/img/university-logo.jpg" alt="university" />
            </education-item>
            <education-item
              src="https://www.dimigo.hs.kr/index.php?mid=class_wp"
              name="한국디지털미디어고등학교"
              period="2013.03 ~ 2016.02 (졸업)"
              description="웹프로그래밍학과"
            >
              <img src="@/assets/img/highschool-logo.jpg" alt="highschool" />
            </education-item>
          </div>
        </content-box>
      </div>
    </div>
  </div>
</template>

<script>
import ContentBox from '@/component/ContentBox.vue';
import EducationItem from '@/component/EducationItem.vue';
import ToggleBox from '@/component/ToggleBox.vue';
import SkillBox from '@/component/SkillBox.vue';

export default {
  name: 'App',
  components: {
    SkillBox,
    ToggleBox,
    EducationItem,
    ContentBox,
  },
};
</script>

<style>
li {
  margin-left: 1rem;
  text-indent: -1.3rem;
}
</style>
