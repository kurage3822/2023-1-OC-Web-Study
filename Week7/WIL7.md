# 클론 코딩

## 유튜브

* 구현 페이지 분석

    * 헤더

    * 영상 재생부

    * 영상 게시자 정보

    * 영상 댓글

    * 추천 영상 목록

* 구획 나누기

    * View (column)

        * header (row)

        * Container (row)

            * main-container (column)

                * video-container

                * video-info-container (column)

                * comment-container (column)

            * aside-container (column)

## 코드

```css
#header {
    position: sticky;
    top: 0;
    padding: 0px 30px;

    background-color: white;
}
```

* position: sticky;

    특정 위치에 고정

* top: 0;

    가장 위에 위치

```css
.grey-bakcground:hover {
    background-color: grey;
    cursor: pointer;
}
```

* hover

    마우스를 올린 경우

* cursor: pointer;

    마우스 커서 변경

```css
#search-bar {
    width: 450px;
    border: 3px solid grey;
    border-radius: 20px;
    padding: 5px 10px;
    color: grey;
    display: flex;
    flex-direction: row;
}
```

* border-radius: 20px;

    테두리 끝을 부드럽게