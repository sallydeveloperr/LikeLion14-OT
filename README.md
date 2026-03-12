# 🦁 Git & GitHub OT 실습

서울여자대학교 멋쟁이사자처럼 14기 **Git & GitHub OT 세션**에서 진행한 Git 기본 실습을 정리한 저장소입니다.

---

# 🦁 1. VCS (Version Control System)

VCS는 **파일의 변경 이력을 관리하는 시스템**입니다.

파일이 언제, 누가, 어떻게 수정되었는지 기록하고  
필요하면 이전 버전으로 되돌릴 수 있도록 해주는 시스템입니다.

Git은 이러한 **버전 관리 시스템(VCS)** 중 하나이며  
**분산 버전 관리 시스템**입니다.

GitHub는 Git으로 관리되는 프로젝트를  
**인터넷에서 저장하고 협업할 수 있도록 도와주는 플랫폼**입니다.

---

# 🦁 2. Git 작업 구조

Git은 다음과 같은 구조로 동작합니다.

```
Working Directory → Staging Area → Local Repository → Remote Repository
```

### 📂 Working Directory
현재 내가 작업하고 있는 실제 파일 위치

### 📂 Staging Area
커밋하기 전에 변경 내용을 임시로 올려두는 공간

### 📂 Local Repository
내 컴퓨터에 저장된 Git 저장소

### 🌐 Remote Repository
GitHub 같은 원격 저장소

---

# 🦁 3. Git 기본 명령어

## 저장소 생성

```bash
git init
```

## 파일 상태 확인

```bash
git status
```

## 파일 추가

```bash
git add .
git add 파일명
```

## 커밋

```bash
git commit -m "커밋 메시지"
```

## 원격 저장소 연결

```bash
git remote add origin [repository URL]
```

## GitHub에 업로드

```bash
git push origin main
```

## GitHub에서 코드 가져오기

```bash
git pull origin main
```

---

# 🦁 4. 협업 시 기본 Git 흐름

협업 시 기본 작업 순서

```
git pull → 코드 수정 → git add → git commit → git push
```

원격 저장소에 새로운 commit이 있는 경우  
**push 전에 반드시 pull을 먼저 해야 합니다.**

---

# 🦁 5. 브랜치를 이용한 협업

브랜치는 기능별 작업을 분리하기 위해 사용합니다.

## 브랜치 생성 및 이동

```bash
git checkout -b 브랜치명
```

작업 후 push하면 GitHub에서 **Pull Request(PR)** 를 생성할 수 있습니다.

Pull Request를 통해 변경사항을 검토한 뒤  
**merge하여 main 브랜치에 반영합니다.**

---

# 🦁 실습 내용

이번 Git OT 실습에서 진행한 과정

1️⃣ GitHub Repository 생성  
2️⃣ 로컬 폴더 생성  
3️⃣ `git init`으로 Git 저장소 초기화  
4️⃣ txt 파일 생성  
5️⃣ `git add` / `git commit` 실행  
6️⃣ `git push`로 GitHub 업로드  
7️⃣ 협업 상황을 가정하여 `git pull` 진행  

---

# 🦁 참고

서울여자대학교 멋쟁이사자처럼 14기  
Git & GitHub OT 세션 자료 기반 정리