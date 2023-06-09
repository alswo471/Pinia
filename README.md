# Pinia

:fire: Pinia 스터디 !! :fire:

<br>

## 소개

<br>

**피니아는 컴포지션 API로 Vue용 스토어가 어떻게 생겼는지 재설계하기 위한 실험으로 시작 했고, Vue2 와 Vue3 모두 작동, API는 설치와 SSR을 제외하고 모두 동일**

<br>

## 피니아 장점

- 피니아는 Vue의 스토어 라이브러리로 컴포넌트/페이지 간에 상태를 공유할 수 있다. 
- Devtools 지원하며, actions, mutations를 추적하는 타임라인, 스토어는 사용되는 컴포넌트에 표시됨. 시간 추적 및 더 쉬운 디버깅
- 핫 모듈 교체 (HMR) 페이지를 새로고침하지 않고 스토어 수정하고, 개발하는 동안 기존 상태 유지
- 플러그인으로 피니아 기능 확장 
- TypeScript 지원 
- SSR 지원

## 왜 피니아인가?

피니아(pinia)는 스페인어 _pineapple_의 영어 발음과 가장 유사한 _piña_입니다.
파인애플은 실제로 각각의 꽃들이 하나의 그룹으로 된 과일입니다.
꽃은 각각 피어나지만, 결국 모두 합쳐지는 모습이 마치 스토어 같습니다.
남아메리카가 원산지인 맛있는 열대 과일이기도 합니다.



## Vuex 와 Pinia 차이점

- 피니아는 더 간단한 API 제공 및 컴포지션 API 스타일 제공, 그리고 TypeScript 지원
- mutations는 존재하지 않음
- 더 이상 매직 문자열을 주입없이, 함수를 가져오고, 호출하고, 자동 완성
- 스토어를 동적으로 추가할 필요가 없
- 더 이상 모듈의 중첩 구조가 없음 그리고  스토어의 순환 종속성을 가질 수도 있음.
- 네임스페이스 모듈이 없고 모든 스토어가 네임스페이스라고 말할 수 있음

<br>

## 시작

<br>

설치 
~~~
yarn add pinia
# 또는 npm으로
npm install pinia
~~~
>앱이 Vue 2.6.x 이하 버전을 사용하는 경우, 컴포지션 API도 설치해야 합니다: @vue/composition-api. Nuxt를 사용하는 경우, 이 지침을 따라야 합니다.

<br>

~~~
import { createApp } from 'vue'
import { createPinia } from 'pinia'
import App from './App.vue'

const pinia = createPinia()
const app = createApp(App)

app.use(pinia)
app.mount('#app')
~~~


<br>
<br>

[출처](https://pinia.vuejs.kr/introduction.html#why-pinia)