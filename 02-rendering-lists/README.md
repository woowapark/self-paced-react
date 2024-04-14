# 02. 목록 UI 구현하기: Props와 State

## 🎯 요구 사항
- `RestaurantList` 가 restaurants 배열을 받아서 그릴 수 있도록 변경해 보세요.
  - restaurants 배열을 `RestaurantList` 의 props로 내려받도록 변경해 보세요.
- 카테고리 필터에 따라 필터된 음식점 목록을 보여줄 수 있도록 변경해 보세요. 

### 구현 결과 예시
```javascript
// App.jsx
<RestaurantList restaurants={restaurants}/>
```

## ✅ 키워드
- Props
- State
  - useState
- Keys

> [Rendering Lists](https://react.dev/learn/rendering-lists) 문서에 ['Why does React need keys?'](https://react.dev/learn/rendering-lists#why-does-react-need-keys)는 지금 꼭 이해하지 않아도 괜찮습니다. 그냥 React에서 목록을 동적으로 그릴 때에는 이런 것들을 사용해야 하는구나~ 정도로만 알고 일단 넘어가세요. 우선 사용하는 법에 익숙해지는 것이 먼저입니다 :) 

## 🧙‍♀️ 진행 가이드
- 진행 시간: 30분 ~ 1시간 내에 완료하는 것을 목표로 합니다. 

## 🔗 참고 문서
- [Thinking in React](https://react.dev/learn/thinking-in-react)의 Step3-4
- [Passing Props to a Component](https://react.dev/learn/passing-props-to-a-component)
- [Rendering Lists](https://react.dev/learn/rendering-lists)
- [State: A Component's Memory](https://react.dev/learn/state-a-components-memory)
  - [API Reference: useState](https://react.dev/reference/react/useState)
