
## for문 과 forEach() 의 차이

#### - 동기(sync), 비동기(async)의 차이

- for문은 동기방식이기 때문에 for문 안에 오류가 나면 에러 위치 이후의 이벤트들은 동작하지 않고 멈춰버린다.
<br/>

#### - 성능 차이

- forEach()는 "향상된 for문"이라 칭하기도 한다. 가변적인 배열이나 리스트 크기를 구할 필요가 없어 복잡한 반복문에 적합하며, 인덱스를 생성하여 접근하는 for문보다 수행속도가 더 빠르다.
-> 내장함수이기 때문
<br/>

## forEach() 단점

- 반복문 내에서 배열이나 리스트 값을 변경하거나 추가할 수 없다. 

- 읽기 전용으로 불러오기 때문에 데이터를 수정하는 행위가 불가능하다.

- 배열을 역순으로 탐색할 수 없다.
<br/>

## JavaScript 에서 forEach() 제어

- 일반적으로 사용하는 for문과 다르게 forEach() 는 함수, 즉 메서드이다. 따라서 반복문이 아닌 함수로 취급되기 때문에 continue와 break를 사용하면 Syntax Error를 내뿜는다.

- forEach()는 각 배열의 각 요소를 단순 순회할 경우 사용, 반복문으로써의 제어가 필요할 경우 for 반복문 사용