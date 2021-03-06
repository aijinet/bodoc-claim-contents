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
3. `git` 으로 배포 이전에 아래의 `금지어 검사` 를 이용하거나 `ctrl`(window) or `command`(mac) + `shift` + `f` 를 이용해 금지어 검색을 실행해 볼 수 있음.
4. `git add .`
5. `git commit -m <your message>`
6. `git push`
7. `git` 에 배포될 때 금지어 검사를 통과하지 않으면 배포를 실패하며 `README.md` 에서 배포 상태를 pass / fall 로 표현.

### 금지어 검사
![ban](https://github.com/aijinet/bodoc-claim-contents/workflows/ban/badge.svg?branch=master)

컨텐츠를 변경하고 이를 `commit` 하거든, 자동으로 금지어 검사가 시작됩니다.

커밋이 완료된 후, 위 뱃지를 눌러 테스트 페이지로 이동해주십시오. 그리고 만일 해당 테스트 페이지에서 금지어가 검출되거든, 뱃지는 빨간색이 될 것이며, 테스트 페이지에서 상세 오류 사유를 확인하실 수 있습니다.

이 금지어 검사는 로컬에서 다음 명령어로도 대신할 수 있습니다. 그리고 금지어 목록은 [assets/config/ban.json](assets/config/ban.json) 에서 관리하실 수 있습니다. 참고로 금지어는 어떻게 입력하던, 대소문자와 띄어쓰기를 무시하고 검사하니, 이 점 유의하시기 바랍니다.

```bash
npm run ban
```