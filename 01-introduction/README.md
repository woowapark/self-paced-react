# 01 Introduction

React는 UI를 렌더링 하기 위한 JavaScript 라이브러리입니다.      
> React is a JavaScript library for rendering user interfaces (UI).
> https://react.dev/learn/describing-the-ui


## ✨ React의 원칙과 목표

React를 사용해 앱을 구현하는 데에는 JavaScript/TypeScript로 앱을 직접 구현하는 것보다는 조금 더 정해진 가이드라인이 있습니다.    
`설계자의 의도`가 그것이죠. React는 새로운 언어나 표준이 아니며, React팀이 그들의 설계 의도에 기반해 만든 하나의 라이브러리입니다.     
사용하는 데에 여전히 정답이 정해져 있지 않은 영역들이 많이 있지만, `권장하지 않는 것`에 대한 가이드는 비교적 명확하게 찾아볼 수 있습니다. 그 가이드는 보통 공식 문서에서 찾을 수 있고요. 이때의 `권장하지 않는 것`들은 그 자체가 잘못되었기 때문이 아니라, `React를 만든 사람들의 의도에서 벗어나기 때문에` 잘못된 것으로 취급됩니다. 즉, 보기에 아주 읽기 좋고 깔끔한 코드라 하더라도 React 팀에서 의도한 설계와 벗어난다면 개발자가 의도하지 않은 동작이 일어날 수도 있고 알 수 없는 버그와 마주할 수도 있다는 뜻입니다.         

즉, 'React를 잘하기 위한 학습'이란 `React에서 의도한 바를 잘 이해하고 그 설계 원칙에 잘 따르는` 코드를 작성하는 법에 대한 학습과 연습이라 할 수 있습니다.      
물론 이 학습의 가장 근본적인 목적은 React를 이해하는 것이 아니라 사용자에게 더 가치있는 서비스를 제공하기 위함이어야 할 것이고요.

### 원칙 
- 1 UI를 컴포넌트 단위로 나누어 구현한다. 각 컴포넌트는 독립적(isolated)이며, 순수함(purity)을 유지해야 한다.
- 2 Single Source of Truth로부터 나온 데이터의 일관성을 유지해야 한다.
- 3 단방향의 데이터 흐름(one-way/unidirectional data flow)을 유지해야 한다.
- 4 선언적 UI

### 목표
위의 원칙을 바탕으로 결국은 여러 측면에서 더 '유지보수하기 좋은'-이미 구현한 걸 파악하고 수정하기 쉬우면서, 확장하기도 쉬운- 코드를 작성하는 것을 목표로 한다.   
- 1 재사용하기 쉬운 (reusable)
- 2 조합하기 쉬운 (composable)
- 3 예측하기 쉬운 (predictable / easy to debug)       

코드를 지향한다. 


> 라이브러리를 학습할 때 해당 라이브러리의 설계 원칙과 목표를 먼저 생각해보는 방식은 React를 학습할 때 뿐만 아니라, 이후에 다양한 상태관리 라이브러리를 학습할 때에도 비슷하게 적용할 수 있습니다.     
> 각각의 라이브러리는 해결하고자 하는 문제가 있으며, 그 문제를 잘 해결하기 위한 과정에서 나름의 설계 원칙을 세우고 원칙에 따라 일관되게 코드를 작성하려 합니다.      
> 영문으로 검색하는 경우 `mental model`, `design principle`, `paradigm` 등을 붙여서 찾아보면 해당 라이브러리에서 지향하는 바에 대한 설명을 찾아볼 수 있습니다. 보통 라이브러리의 공식 문서, 라이브러리 컨트리뷰터들이 작성한 아티클 혹은 컨퍼런스 발표 등에서 찾아볼 수 있어요. 이 자료에서 확인할 수 있는 원칙들이 말 그대로 '저자의 의도'이니 가장 정확한 가이드라인이라 할 수 있습니다.       

## 🦅 공식 문서 Overview 
[React 공식 문서](https://react.dev/)에서 필요한 대부분의 학습 자료를 모두 찾을 수 있습니다. 설계 원칙부터 사용법, 연습 문제를 직접 풀어볼 수 있는 IDE까지 내장되어 있으니 가능하면 공식 문서를 활용해 학습해보는 연습을 추천합니다.       

공식 문서는 크게 아래와 같은 구성으로 이루어져 있습니다.            
- Learn
- Reference
	- API Reference
		- Reference
		- Usage
		- Troubleshooting
	- Rules of React

Self-Paced React에서 연습용 앱의 각 단계별 요구 사항을 구현할 때 참고할 만한 공식 문서 링크를 몇 개씩 함께 달아두었습니다. 


## 권장하는 학습 단계
이 자료는 JavaScript/TypeScript로 간단한 애플리케이션을 구현해보았지만 React는 아직 학습해본 적 없는 크루를 대상으로 합니다.    
- 1 Self-Paced React: React를 사용해 '일단 돌아가게 하는 법'을 연습해본다. 
- 2 우아한테크코스 레벨2 미션&피드백: React를 '잘' 활용하는 법, 'React다운' 코드를 쓰는 방법을 좀 더 복잡한 UI를 완성도 높게 구현해보면서 연습한다. 그게 '왜' 잘 쓰는 법인지를 공식 문서 기준으로 학습한다.
- 3 optional: 잘 활용하는 것을 넘어서서 더 깊은 동작 원리를 학습한다.

## 시작 전 워밍 업
[Quick Start](https://react.dev/learn) 페이지의 내용을 차근차근 따라해 보세요. 아주 간단한 React 사용법을 전반적으로 알아볼 수 있습니다.     

대략적인 React 코드의 생김새에 익숙해졌나요? 
[Thinking in React](https://react.dev/learn/thinking-in-react)를 읽으며 UI를 React로 구현하는 과정을 살펴보세요. Self-Paced React 에서 구현해볼 작은 앱도 이 [Thinking in React](https://react.dev/learn/thinking-in-react) 문서에서 가이드하는 흐름을 참고해 단계별 요구 사항을 제시할 예정입니다.        

[Thinking in React](https://react.dev/learn/thinking-in-react) 문서까지 살펴봤다면, 다음 단계로 넘어가 주세요. (이 문서의 모든 것을 이해해야 한다는 뜻은 아닙니다! 가볍게 훑어보고 넘어가세요. 지금 모든 걸 이해하지 않아도 괜찮습니다.)

## 참고: React(core)와 React Renderer의 관계 
`main.jsx`파일을 한번 열어보세요. 아래와 같은 import 문이 있는 것을 확인하실 수 있습니다. 
```javascript
import React from "react";
import ReactDOM from "react-dom/client";
```
거칠게 나눠보자면 React로 애플리케이션을 구현할 때에는 React(core)와 React Renderer를 함께 사용하게 됩니다. `ReactDOM`이 React renderer의 한 종류로 웹 브라우저 환경에서 React코드를 실행하기 위해 사용합니다.        

![react and react renderers](../images/01-react-react-renderers.jpg)        

실제로 React Native를 처음 소개할 때에는 [`Learn once, write everywhere`](https://blog.outsider.ne.kr/1124) 라는 슬로건을 내세우기도 했습니다. (정말로 이 슬로건을 잘 실현했는지는 일단 논외로 두겠습니다)      

흔히 접할 수 있는 ReactDOM이나 React Native 외에도, [awesome react renderer](https://github.com/chentsulin/awesome-react-renderer)를 보시면 작성한 React 코드를 다양한 환경에서 실행시킬 수 있는 React Renderer들을 확인할 수 있고, 심지어는 직접 Renderer를 구현할 수도 있습니다.      

이 자료에서는 React Renderer, React Core와 React Renderer의 연결 구조와 관련한 더 깊은 이해를 위한 설명은 제외합니다.      
앞으로의 자료에서는 이러한 전체적인 구조와 깊은 동작 원리보다는 우선 React 자체를 사용해 코드를 작성하는 것에 대한 부분을 다룹니다. 
