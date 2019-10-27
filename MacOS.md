# MacOS

현재 사용중인 컴퓨터의 운영체제가 MacOS인데, 처음 개발을 공부할 때 개발도 물론이거니와 이 맥이라는 환경에 개발자로서 적응해야하는 시간도 필요했다. 그래서 공부하면서 알게 된 것들을 정리해 남겨보겠다.

- [Homebrew](#homebrew)
- [tree 패키지](#osx-package-tree)

<br>

## <a name="homebrew"></a>Homebrew

<img src="http://www.mediafire.com/convkey/011a/ug38gl0hjk0f0s1zg.jpg" width="500" />

[Homebrew](https://brew.sh/index_ko)는 맥OS 또는 리눅스에서 기본으로 제공하지 않는 패키지를 설치/제거할 수 있는 패키지 관리자다. 리눅스의 `apt-get` 과 비슷한 역할을 한다.

보통 맥에서 필요한 패키지를 설치할 때 자주이용하는 서비스니 맥을 사용하는 개발자라면 익혀두면 좋다.

### Homebrew 설치

터미널을 열고 아래 명령어를 붙여넣기하고 입력하면 homebrew가 설치된다. 엄청 간단하다.

`/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`



### 패키지 설치

설치하고 싶은 패키지가 있다면, 먼저 패키지가 있는지 알아둬야 한다.

`brew search [package-name]`

있다면 `search` 대신 `install`로 바꾸어서 패키지를 설치하면 된다.

`brew install [package-name]`



### homebrew 업데이트

기본적으로 패키지를 설치하기 전에 homebrew가 자동으로 업데이트를 진행하지만, 일단 알아두자.

`brew update`

<br>

## <a name="osx-package-tree"></a>Tree 패키지

터미널에서 디렉토리를 계층적으로 분리해서 볼 수 있는 패키지다.

깃헙에서 사용할 수 있는 익스텐션인 [Octotree](https://www.octotree.io/)와 비슷하다.



### 패키지 설치

[homebrew](#homebrew)를 이용해서 설치할 수 있다. 

`brew install tree`



### 패키지로 디렉토리 한 눈에 보기

현재 디렉토리를 터미널에서 계층적으로 구분해서 편하게 보려면 `tree .` 을 입력하면 된다.

<img src="http://www.mediafire.com/convkey/0813/u5n9x04o217pgqezg.jpg" width="500" />

<br>