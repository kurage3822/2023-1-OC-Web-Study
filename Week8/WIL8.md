# 기본 문법

## JS

* 선언

    * 변수

        ```js
        var x;
        ```

        var 키워드를 사용

        데이터 타입을 미리 지정하지 않음

    * 함수

        ```js
        function square(number)
        {
            return number * number;
        }
        ```

        function 키워드를 사용

    * 배열

        ```js
        var arr = [1, 2, 3, 4, 5];
        ```

        대괄호를 사용

* 데이터 타입

    * 정수와 실수

        ```js
        console.log(1 === 1.0); // true
        console.log(3 / 2);     // 1.5
        ```

        정수만을 위한 타입이 없고 모든 수를 실수로 처리

        정수의 나눗셈의 결과도 몫이 아닌 실수

    * 특별한 값들

        ```js
        console.log(10 / 0);        // Infinity
        console.log(10 / -0);       // -Infinity
        console.log(1 * 'string');  // NaN
        ```

        Infinity : 양의 무한대

        -Infinity : 음의 무한대

        NaN : 산술 연산 불가(not-a-number)

    * 문자열의 값 변경

        ```js
        var str = 'string';
        str[0] = 'S';
        console.log(str); // string

        str = 'String';
        console.log(str); // String
        ```

        이미 생성된 문자열의 일부 문자를 변경해도 반영되지 않음

        새로운 문자열을 재할당하는 것은 물론 가능

    * undefined

        ```js
        var foo;
        console.log(foo); // undefined
        ```

        선언 이후 값을 할당하지 않은 변수의 값

* 변수 호이스팅(Variable Hoisting)

    ```js
    console.log(foo); // ① undefined

    var foo = 123;
    console.log(foo); // ② 123

    {
    var foo = 456;
    }
    console.log(foo); // ③ 456
    ```

    모든 선언문이 해당 Scope의 선두로 옮겨진 것처럼 동작하는 특성

* 연산자

    * 비교

        * == (동등)

            ```js
            5 == '5' // true
            ```

            암묵적 타입 변환을 통해 타입을 일치시킨 후 같은 값을 갖는지 비교

            ```js
            0 == ''             // true
            0 == '0'            // true
            '' == '0'           // false

            false == 'false'    // false
            false == '0'        // true

            false == undefined  // false
            false == null       // false
            null == undefined   // true
            ```

            예측하기 어려운 결과를 만들어낼 가능성이 존재

        * === (일치)

            ```js
            5 === '5' // false
            ```

            타입도 같고 값도 같은 경우에 한하여 true를 반환

            ```js
            NaN === NaN // false
            ```

            NaN은 자신과 일치하지 않는 유일한 값

            ```js
            isNan(NaN) // true
            ```

            숫자가 NaN인지 조사하려면 빌트인 함수 isNaN을 사용

    * 논리

        * 합과 곱

        ```js
        // 단축 평가
        'Cat' && 'Dog' // 'Dog'
        'Cat' || 'Dog' // 'Cat'
        ```

        언제나 피연산자 중 어느 한쪽 값을 반환

## ES6

* let

    ```js
    let foo = 123;      // 전역 변수

    {
    let foo = 456;      // 지역 변수
    let bar = 456;      // 지역 변수
    }

    console.log(foo);   // 123
    console.log(bar);   // ReferenceError: bar is not defined
    ```

    블록 레벨 스코프를 따르는 변수를 선언하기 위해 let 키워드를 제공

    ```js
    let bar = 123;
    let bar = 456;  // Uncaught SyntaxError: Identifier 'bar' has already been declared
    ```

    변수를 중복해서 선언할 수 없음

    ```js
    console.log(bar); // Error: Uncaught ReferenceError: bar is not defined
    let bar;
    ```

    스코프의 시작에서 변수의 선언까지 일시적 사각지대(Temporal Dead Zone; TDZ)에 빠짐
