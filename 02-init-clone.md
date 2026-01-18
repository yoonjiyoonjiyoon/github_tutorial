# 저장소 생성과 클론

## 저장소를 만들고, 외부 저장소를 불러오는 법
### git init 이란?
git init은 현재 디렉토리를 Git 저장소로 초기화하는 명령어이다.
이 명령을 실행하면 해당 디렉토리는 Git의 버전 관리 대상이 되며, 이후 파일 변경 이력과 커밋을 기록할 수 있다.
주로 새 프로젝트를 처음 시작할 때 사용된다.

### git clone 이란?
git clone은 원격 저장소를 로컬 저장소로 그대로 복사하는 명령어이다.
프로젝트의 파일뿐 아니라 커밋 이력, 브랜치 구조까지 함께 가져오며,
이미 존재하는 GitHub 프로젝트에 참여할 때 사용된다.
> 원격저장소를 로컬저장소로.

### fork란?
Fork는 다른 사용자의 원격 저장소를 자신의 GitHub 계정으로 복사하는 기능이다.
원본 저장소에 직접 수정 권한이 없을 때 사용되며,
복사된 저장소에서 자유롭게 작업한 후 변경 사항을 Pull Request로 제안할 수 있다.
주로 **오픈소스 프로젝트 기여**나 **권한이 없는 저장소에 대한 협업**에서 사용된다.
> 원격저장소를 원격저장소로.

### git config 이란?
git config는 Git의 사용자 정보 및 동작 설정을 관리하는 명령어이다.
대표적으로 커밋 작성자를 식별하기 위한 사용자 이름과 이메일을 설정하며,
이 정보는 모든 커밋 기록에 포함된다.

## 용례
### git init
![alt text](/img/그림2.png)
```sh
git init
```
git init 명령어가 수행하는 것은 엄밀히 말하면 ~

### git clone
![alt text](/img/그림1.png)
```sh
git clone https://github.com/username/repository.git #<URL>.git
```
git clone 을 통해서 웹사이트의 저장소를 자신의 로컬 저장소를 불러 올 수 있다.

### fork
![alt text](/img/그림3.png)
fork로 타인의 원격 저장소의 repo를 자신의 원격 저장소를 불러 올 수 있다.
응용한다면, fork후 자신의 원격 레포지 토리에서 clone 하여 

### git config
```sh
git config --global user.name "YOUR_NAME"
git config --global user.email "YOUR_EMAIL"
```