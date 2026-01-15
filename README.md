# 퍼포먼스 대시보드 모음

## GitHub Pages 배포 방법 (상세 가이드)

### 1단계: 새 저장소 생성

1. [GitHub](https://github.com)에 로그인
2. 우측 상단의 **"+"** 버튼 클릭 → **"New repository"** 선택
3. 저장소 이름 입력 (예: `dashboard-totalDB` 또는 `performance-dashboard`)
4. **Public** 선택 (GitHub Pages는 Public 저장소에서 무료)
5. **"Add a README file"** 체크 해제 (이미 README.md가 있으므로)
6. **"Create repository"** 클릭

### 2단계: 파일 업로드

**방법 A: 웹에서 직접 업로드 (간단)**

1. 생성된 저장소 페이지에서 **"uploading an existing file"** 클릭
2. `index.html` 파일을 드래그 앤 드롭
3. 하단에 커밋 메시지 입력 (예: "Initial commit")
4. **"Commit changes"** 클릭

**방법 B: Git 명령어 사용 (고급)**

터미널에서 다음 명령어 실행:

```bash
cd C:\Users\AC0734\Desktop\dashboard\totalDB
git init
git add index.html README.md
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/[사용자명]/[저장소명].git
git push -u origin main
```

### 3단계: GitHub Pages 활성화

1. 저장소 페이지에서 **"Settings"** 탭 클릭
2. 왼쪽 메뉴에서 **"Pages"** 클릭
3. **"Source"** 섹션에서:
   - Branch: **"main"** 선택
   - Folder: **"/ (root)"** 선택
4. **"Save"** 클릭

### 4단계: 배포 완료

1. 몇 분 후 (보통 1-2분) 페이지 새로고침
2. **"Pages"** 설정 페이지 상단에 초록색 체크 표시와 함께 URL이 표시됨
3. URL 형식: `https://[사용자명].github.io/[저장소명]/`
   - 예: `https://yourusername.github.io/dashboard-totalDB/`

### 5단계: 공유하기

생성된 URL을 다른 사람들에게 공유하면 됩니다!

---

## 주의사항

- 저장소 이름에 대문자나 특수문자가 있으면 URL에 그대로 반영됩니다
- 첫 배포 후 변경사항이 있으면 파일을 다시 업로드하고 커밋하면 자동으로 업데이트됩니다
- 배포에는 보통 1-2분 정도 걸립니다

### 방법 2: Netlify (가장 간단)

1. [Netlify](https://www.netlify.com) 접속
2. "Add new site" > "Deploy manually"
3. `index.html` 파일을 드래그 앤 드롭
4. 즉시 URL 생성됨 (예: `https://random-name-123.netlify.app`)

### 방법 3: Vercel

1. [Vercel](https://vercel.com) 접속
2. "Add New Project"
3. `index.html` 파일 업로드
4. 즉시 URL 생성됨

### 방법 4: 단순 파일 공유

- Google Drive, Dropbox, OneDrive 등에 업로드
- 공유 링크 생성
- 단점: 직접 파일 다운로드 필요

## 로컬에서 테스트

파일을 더블클릭하거나 브라우저에서 열면 바로 확인 가능합니다.

