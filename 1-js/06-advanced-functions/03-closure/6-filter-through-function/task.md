importance: 5

---
# 필터 통과 기능
우리는 어레이를 위한 `arr.filter (f)` 라는 내장 메서드를 가지고 있습니다. 이 함수는 `f` 함수를 통해 모든 요소를 필터링합니다. `true` 를 돌려주는 경우, 결과의 배열에 그 요소가 반환됩니다.

"사용할 준비가 된" 필터 세트 만들기 :

- `inBetween(a, b)` -- a와 b 또는 그와 동등한 것 (포함)
- `inArray([...])` -- 주어진 배열에서

사용법은 다음과 같아야 합니다:

- `arr.filter(inBetween(3,6))` -- 3과 6 사이의 값만 선택합니다.
- `arr.filter(inArray([1,2,3]))` -- `[1,2,3]`의 멤버 중 하나와 일치하는 요소만 선택합니다.

예를 들면 :

```js
/* .. 사이 및 배열에 대해 당신을 위한 코드 */
let arr = [1, 2, 3, 4, 5, 6, 7];

alert( arr.filter(inBetween(3, 6)) ); // 3,4,5,6

alert( arr.filter(inArray([1, 2, 10])) ); // 1,2
```

