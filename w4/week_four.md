# Week 4

### AMEND COMMITS

- 가장 최근 커밋을 수정
  - 메세지 수정:
    - `git commit --amend -m "message"`
  - 메세지 유지:
    - `git commit --amend --no-edit`

### [IGNORING FILES](https://mygumi.tistory.com/103)

- `.gitignore` 파일 생성
  - 커밋하고 싶지 않은 파일/폴더를 넣으면 해당 파일/폴더는 트랙되지 않고 커밋되지 않음
    - 파일: 파일이름 ➡️ .env
    - 폴더: /폴더이름 ➡️ /images
- `.gitignore` 생성 전에 무시하고 싶은 파일/폴더를 **커밋** 했다면

  - **원격 저장소와 로컬 저장소**에 있는 파일을 삭제

    1. `git rm file` ➡️ `git rm .env`
    2. `git rm -r folder` ➡️ `git rm -r images/`

  - **원격 저장소**에 있는 파일을 삭제

    1. `git rm file --cached`
    2. `git rm -r folder --cached`

### ORIGINS

- 깃헙 외 원격 저장소 사용하기 (bitbucket, gitlab, etc.)
- 원격 저장소 목록 보기
  - `git remote -v`
- 원격 저장소 추가하기
  - `git remote add gitname url`
    - `git remote bitbucket https://~`
- 추가한 원격 저장소에 푸시
  - `git push gitname main`
    - `git push bitbucket main`
- 원격 저장소 삭제하기
  - `git remote remove gitname`
    - `git remote remove bitbucket`
