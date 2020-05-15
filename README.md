# BODOC CLAIM CONTENTS
![ban](https://github.com/aijinet/bodoc-claim-contents/workflows/ban/badge.svg?branch=master)

## Purpose

   - Provide information about Claims

## Installation

```bash
# Get source from repository
git clone https://github.com/aijinet/bodoc-claim-contents.git
cd bodoc-claim-contents
# If you installed VSCode
code .
```

## Usage
### Initial
1. `contents` 폴더 안에 md 파일을 저장할 구조에 맞게 폴더를 생성
2. 생성한 폴더 내에 md 파일을 작성 및 저장
3. `git remote add origin https://github.com/aijinet/bodoc-claim-contents.git`
4. `git add .`
5. `git commit -m <your message>`
   - example) `git commit -m "first commit"`
6. `git push --set-upstream origin <your branch>`
   - example) `git push --set-upstream origin https://github.com/aijinet/bodoc-claim-contents.git`

### Normal
1. `contents` 폴더 안에 md 파일을 저장할 구조에 맞게 폴더를 생성
2. 생성한 폴더 내에 md 파일을 작성 및 저장
3. `npm run ban` 를 이용해 자동 필터링 기능을 사용해 보거나 `ctrl`(window) or `command`(mac) + `shift` + `f` 를 이용해 금지어 검색을 실행해 볼 수 있음.
4. `git add .`
5. `git commit -m <your message>`
6. `git push`
7. 푸시가 완료되고 레파지토리의 Reamme.md 파일을 웹에서 확인하면 현재 상태가 pass / fall 했는지 알 수 있다.