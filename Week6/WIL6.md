# Flexbox

## justify-content

* flex-start

    요소들을 컨테이너의 왼쪽으로 정렬

* flex-end

    요소들을 컨테이너의 오른쪽으로 정렬

* center

    요소들을 컨테이너의 가운데로 정렬

* space-between

    요소들 사이에 동일한 간격을 둠

* space-around

    요소들 주위에 동일한 간격을 둠

## align-items

* flex-start

    요소들을 컨테이너의 꼭대기로 정렬

* flex-end

    요소들을 컨테이너의 바닥으로 정렬

* center

    요소들을 컨테이너의 세로선 상의 가운데로 정렬

* baseline

    요소들을 컨테이너의 시작 위치에 정렬

* stretch

    요소들을 컨테이너에 맞도록 늘림

## flex-direction

* row

    요소들을 텍스트의 방향과 동일하게 정렬

* row-reverse

    요소들을 텍스트의 반대 방향으로 정렬

* column

    요소들을 위에서 아래로 정렬

* column-reverse

    요소들을 아래에서 위로 정렬

## flex-wrap

* nowrap

    모든 요소들을 한 줄에 정렬

* wrap

    요소들을 여러 줄에 걸쳐 정렬

* wrap-reverse

    요소들을 여러 줄에 걸쳐 반대로 정렬

## flex-flow

공백문자를 이용하여 flex-direction, flex-wrap, 두 속성의 값들을 인자로 받음

# Flexbox Froggy 답

-1- justify-content: flex-end;

-2- justify-content: center;

-3- justify-content: space-around;

-4- justify-content: space-between;

-5- align-items: flex-end;

-6- justify-content: center; align-items: center;

-7- justify-content: space-around; align-items: flex-end;

-8- flex-direction: row-reverse;

-9- flex-direction: column;

-10- flex-direction: row-reverse; justify-content: flex-end;

-11- flex-direction: column; justify-content: flex-end;

-12- flex-direction: column; justify-content: space-between;

-13- flex-direction: row-reverse; justify-content: center; align-items: flex-end;

-18- flex-wrap: wrap;

-19- flex-direcion: column; flex-wrap: wrap;

-20- flex-flow: column wrap;