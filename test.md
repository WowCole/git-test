## Git 실습 - 문제풀기
> 아래에 있는 각각의 문제에 대해 답과 이유를 작성하시오.
> 함께 PR을 날리면서 집단지성을 통해 문제를 풀어 봅시다.

1. git은 무엇인가요?   
   - 답 : 버전 관리 시스템으로 분산적으로 작업하는 병렬 개발이 가능하다
  
2. Staging Area의 역할은 무엇일까요?
   - 답 :  커밋하기 위해 git add 명령어로 추가한 파일들이 모여있는 공간

3. 변경사항을 기록하는 과정을 아래 코드 블록에 작성해 주세요.
   - 답
   ```bash
    ## 저장 이후
    $git add .
    $git commit -m <"변경 기록 사항">
    $git push origin <브랜치나 마스터> (github 에 반영하기 위해)
  
   ```

4. 아래와 같은 메시지가 발생했을 때, 무엇을 해야 할까요?
![image](https://user-images.githubusercontent.com/98133984/181182281-4d01a374-62fe-4957-9a07-1efc005e35d3.png)
   - 답
   ```bash

    $git config --global user.name "이름"
    $git config --global user.email "메일 주소"

   ```
5. clone과 pull의 차이는 무엇인가요?
   - 답 : clone 은 복사 pull은 동기화 
   
6. branch를 만드는 목적은 무엇인가요?
    - 답 : 작업 공간을 나누어 독립적으로 작업이 가능하기 때문에 원본에 대해 안전하고 체계적인 개발이 가능하다 오류나 버전을 수정하여 적용할때 확실한 기록이 될 수 있고 혹여 잘못되더라도 어디에서 잘못된것인지 어떻게 되돌릴것인지 쉽게 파악하고 수정이 가능하다.

7. branch를 생성하는 동시에 이동하는 명령어는 무엇인가요?
    - 답 : git switch -c <이름>

8. 다음과 같은 상황이 나타났을 때 어떻게 해야 하나요?
   ![image](https://user-images.githubusercontent.com/98133984/181183354-df42d325-b839-48e1-a4c6-667c20b33d5c.png)
    - 답 :원격저장소에 local 에 없는 자료가 있을때 나타나며 pull 을 사용하여 업데이트 하고 난 뒤 다시 푸시하면 해결된다.

9.  소유권이 없는 협업을 하기 위해서 가장 먼저 해야 할 것은 무엇일까요?
    - 답 : fork  
10. 소유권이 없는 협업의 경우, `git push origin master`로 원격 저장소에 변경사항을 반영할 수 있다.
    - 답 : X
    - 이유 :fork 를 통해 요청해야한다.
 
11. git reset 명령어의 옵션 중, staging area 상태로 돌아가는 옵션은 ______이다.
    - 답 : git reset --soft

12. 바로 직전 커밋을 수정하기 위해서 필요한 명령어를 작성하세요.
    - 답
    ```bash
    git commit --amend
    ```

13. merge와 rebase의 차이점은 무엇일까요? 
     - 답 : 
