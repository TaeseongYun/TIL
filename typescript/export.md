ES6 부터 import export 를 해주며 손쉽게 모듈을 가져오고 내보낼 수 있게되었다.
자세히 알아보자.

export로 함수, 객체, 값을 내보내고 import로 가져다 쓴다.

# Export

export를 하는 방법에는 두 가지가 있다.
named 내보내기, default 내보내기.

- export named ?

```typescript
//먼저 선언한 함수 내보내기
export { myFunction };
//상수 내보내기
export const foo = Math.sqrt(2);
```

- export default ?

```typescript
//기본 내보내기
export default function () {}

//클래스 내보내기
export default class {}
```

### 차이점

- export default 는 하나의 파일에 하나만 가능하다.

- named export 는 동일한 이름으로 가져올 수 있고 as 키워드로 변경 가능하다.
