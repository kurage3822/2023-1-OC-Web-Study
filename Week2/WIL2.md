# 필수 과제

## git의 명령어 add, commit, push, pull, fetch

* add

    working directory 상의 변경 내용을 staging area에 추가

* commit

    staging area에 있는 변경 내용들을 .git에 저장

* push

    remote repository에 .git을 업로드

* pull

    remote repository의 소스를 fetch와 merge 명령어를 사용하여 가져옴

* fetch

    소스를 가져옴

* pull과 fetch의 차이점

    pull은 소스를 가져와서 merge를 하고 fetch는 merge를 하지 않음

## WIL1, WIL2

### WIL1

* URI (Uniform Resource Identifier)

    통합 자원 식별자로 인터넷의 자원을 식별할 수 있는 문자열

* URL (Uniform Resource Location)

    프로토콜 + DNS 주소로 구성

* URN (Uniform Resource Name)

* DNS (Domain Name Server)

    호스트의 도메인 이름을 호스트의 네트워크 주소로 바꾸거나 그 반대의 변환을 수행

브라우저는 HTML, CSS, JS를 재료 삼아 렌더링함

* HTML

    자료 (뼈대)

* CSS

    UI (살과 옷)

* JavaScript

    제어

### WIL2

* Git

    컴퓨터 파일의 변경사항을 추적하고 여러 명의 사용자들 간에 해당 파일들의 작업을 조율하기 위한 분산 버전 관리 시스템

* 깃이 관리하는 파일의 4가지 상태

    1. Untracked
    2. Unmodified
    3. Modified
    4. Staged

* Working Directory

    작업 공간

* Staging Area

    변경 내용을 쌓아두는 공간
    git add 명령어를 통해 쌓을 수 있음

* Local Repository

    커밋을 마친 코드가 저장되는 저장소

* Remote Repository

    git의 변화 데이터들을 모아둘 수 있는 곳인 외부 저장소
    Github도 이러한 서비스 중 하나

# 선택 과제

Unity Hub에서 프로젝트를 만들어 commit을 하려고 했더니 파일 크기 제한 경고가 뜸

.gitignore을 작성하여 불필요한 파일을 제외하는 것으로 문제를 해결