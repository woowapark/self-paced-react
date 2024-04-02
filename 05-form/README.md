
# 🎯 요구 사항
- GNB의 레스토랑 추가 버튼을 클릭하면 레스토랑 추가 폼이 모달로 뜨도록 구현해 주세요
  - (작은 단계로 구현해보기 1) 이전 단계에서 만든 레스토랑 상세 정보 모달을 쓰지 않고 레스토랑 추가용 모달을 따로 만들어서 띄웁니다.
  - (작은 단계로 구현해보기 2) 이전 단계에서 만든 모달을 재사용하여 구현합니다. 
- `<input/>`, `<textarea/>`에 값을 입력하고 '확인' 버튼을 클릭하면 레스토랑 목록에 추가되도록 구현해 주세요. 
  - 유효성 검사는 하지 않습니다. 아주 간단하게 입력값을 처리해보는 구현만 해도 충분합니다.

# 🔗 참고 문서
- [Sharing State Between Components](https://react.dev/learn/sharing-state-between-components)

# ✅ 키워드
- lifting state up
- controlled vs uncontrolled
- children props

> 재사용할 수 있는 모달을 만들 때 `children`을 활용해 보세요. 아래와 같은 식으로 UI를 구성할 수 있습니다.      

```javascript
// 레스토랑 추가 모달 
<Modal>
  // 설명을 위한 예시용 마크업입니다. 실제로 사용하는 마크업은 template/ 하위의 html을 참고하거나 직접 원하는대로 구현하여 사용해 주세요.
  <label></label>
  <input />
  <label></label>
  <textarea />
</Modal>

// 레스토랑 정보 모달 
<Modal>
  // 설명을 위한 예시용 마크업입니다. 실제로 사용하는 마크업은 template/ 하위의 html을 참고하거나 직접 원하는대로 구현하여 사용해 주세요.
  <h2></h2>
  <p></p>
</Modal>
```
