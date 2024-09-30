# Intersection Observer를 이용한 무한 스크롤 구현
2024 원티드 프리온보딩 FE 챌린지 사전 과제로 무한 스크롤을 구현하였습니다.<br/>
[사전과제 요구사항 링크](https://gist.github.com/goldfrosch/034b966075059447efa1c00476849d68)

### 실행 방법
1. 프로젝트 clone
2. `npm install`
3. `npm start`

## 구현 결과
https://github.com/user-attachments/assets/e2d86193-773d-4f1b-93d0-37cd53133ad4

## 핵심 아이디어
1. Intersection Observer API는 루트 요소를 스크롤하다 타겟 요소를 만나면 callback을 실행하는 API입니다.
2. 루트로 지정할 요소, 그리고 타겟 요소가 어느 정도 보일 때 callback을 실행할 지 비율을 다음과 같이 지정해줄 수 있습니다.
```javascript
const options = {
    root: document.querySelector('.App-main'), // 루트로 지정할 요소
    rootMargin: '0px',
    threshold: 0.5, // (0~1 사이값, 배열 지정 가능)
  }
```

3. 옵저버 할당
4. 타겟 지정
5. 옵저버 해제

작성중...
