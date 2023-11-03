# Week 3

### [Terminal Commands](../commands.md)

---

### M과 U의 차이

- VS Code에서 파일 옆에 M과 U 아이콘들은 무엇인가?

    <img src="../imgs/w3/01.png" width="250">

  - **M = Modified**
    - 깃이 관찰하고 있는 파일이 수정 되었을 때
  - **U = Untracked**
    - 아직 깃에서 등록되지 않아 관찰되고 있지 않은 파일
    - 커밋을 해야 등록/관찰이 됨

---

### COMMIT HISTORY

- 개발자가 여태 커밋한 기록을 보는 것

  1. `git log`

     <img src="../imgs/commands/01.png" width="500">

     - `commit # (HEAD -> main)` = 내 컴퓨터
       - 마지막 커밋은 이전 커밋의 내용들이 다 합쳐져 있음
     - `commit # (origin/man)` = 깃헙 저장소

      <img src="../imgs/commands/02.png" width="500">

     - `commit # (HEAD -> main, origin/man)` = 내 컴퓨터와 깃헙 저장소가 같은 커밋에 있음

  2. `q`

  - `git log` 에서 탈출하기

---

### HEAD

- 지금 시점에 파일이 있는 위치
- HEAD의 위치를 변경하여 이전 파일 변경사항을 볼 수 있음
  - `git checkout #`
    - git checkout d7aa16ae5e4d46d529292e027934e727de9e4298
