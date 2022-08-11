## ***💣 git pull = git fetch + git merge***

pull과 fetch의 차이점은 병합을 하냐 안 하냐의 차이다.

## ***1. git pull ?***

**원격저장소에 있는 프로젝트의 변경사항을 그대로 로컬저장소에 옮겨와 자동으로 병합**팀 단위로 사용하는 계정이 아닌 개인적으로 깃허브를 사용하는 사람들이라면 git pull 명령어를 가장 많이 사용할 것이다.***"변경 사항을 가져옴과 동시에 자동으로 병합이 되기 때문에 무엇이 추가되고 병합되었는지 확인이 안 됨"***

## ***2. git fetch ?***

**원격저장소에 있는 프로젝트의 변경사항을 가져오기만 한 후 병합(merge)은 따로**깃 입문자 또는 깃허브를 개인적으로 사용하는 사람이라면 git fetch 명령어는 거의 사용하지 않을 것이다.**"다른 사람이 수정한 부분을 확인하고 병합할 수 있다는 장점이 있음"**

## ***3. git clone ?***

**clone이라는 단어처럼 원격저장소의 내용을 새로운 폴더에 그대로 복사하는 것!**

 push한 최신 작업본을 사용하기 위해 깃헙에서 master 브랜치를 pull합니다.
위에서 말씀드린 대로 승수, 성훈님은 pull할 때 master 브랜치로 이동한 후, pull하도록 합니다.
브랜치를 이동할 때, 작업을 마무리 짓고 commit을 한 후 이동해야 합니다. ( working directory에 작업내용이 있다면 브랜치 이동이 안됩니다. )

```java
git checkout master
git pull origin master
```

최신 버전을 가져왔으면, 자신의 작업본에 반영해야 합니다.

승수님을 기준으로 말씀드리면, brchA 브랜치로 이동 후 master 브랜치를 merge하면 됩니다.

```java
git checkout brchA
git merge master
```