# Git 저장소 연결 가이드

## 1단계: GitHub에서 저장소 생성

1. [GitHub](https://github.com) 로그인
2. 우측 상단 **"+"** → **"New repository"**
3. 저장소 이름 입력 (예: `performance-dashboard`)
4. **Public** 선택
5. **"Add a README file"** 체크 해제 ⚠️
6. **"Create repository"** 클릭

## 2단계: 로컬 폴더와 연결

저장소 생성 후 GitHub에서 표시되는 페이지에서 **"…or push an existing repository from the command line"** 섹션을 찾으세요.

아래 명령어를 순서대로 실행하세요:

```bash
# 1. Git 저장소 초기화
git init

# 2. 모든 파일 추가
git add .

# 3. 첫 커밋
git commit -m "Initial commit"

# 4. main 브랜치로 이름 변경
git branch -M main

# 5. GitHub 저장소 연결 (여기서 [사용자명]과 [저장소명]을 실제 값으로 변경!)
git remote add origin https://github.com/[사용자명]/[저장소명].git

# 6. GitHub에 푸시
git push -u origin main
```

## 예시

만약 GitHub 사용자명이 `john`이고 저장소명이 `performance-dashboard`라면:

```bash
git remote add origin https://github.com/john/performance-dashboard.git
```

## 3단계: GitHub Pages 활성화

1. GitHub 저장소 페이지에서 **"Settings"** 탭 클릭
2. 왼쪽 메뉴에서 **"Pages"** 클릭
3. **Source**: Branch를 **"main"**, Folder를 **"/ (root)"** 선택
4. **"Save"** 클릭
5. 1-2분 후 URL 생성됨: `https://[사용자명].github.io/[저장소명]/`

## 이후 업데이트 방법

파일을 수정한 후:

```bash
git add .
git commit -m "업데이트 내용 설명"
git push
```

자동으로 GitHub Pages에 반영됩니다!


