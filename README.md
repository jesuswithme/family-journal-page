# Family Journal Page

사진 3장과 주제에서 감성적인 한국어 글과 카피를 작성하고, 원본 사진을 활용해 가족 라이프 저널 페이지를 만드는 Claude Code 스킬입니다.

## 기능
1. 사진 3장 검토 및 대표 사진 선택
2. 대표 제목, 부제, 사진별 카피 3개, 감성적인 본문 작성
3. 원본 사진 1장 크게 + 2장 작게 배열한 저널 이미지 제작
4. 한글·이름·날짜 검수

기본 스타일은 크림색 종이 질감, MUJI/Kinfolk 계열 미니멀 에디토리얼, 붓글씨 제목, 자연스러운 여백입니다.

> **원본 사진 보존:** 이미지 생성 모델은 얼굴이나 한글을 바꿀 수 있습니다. 원본 사진을 정확히 보존해야 한다면 이미지 생성 대신 실제 사진을 직접 캔버스에 합성하는 방식이 우선입니다. 이미지 제작에는 별도의 이미지 생성·편집 기능이 필요합니다.

## 설치

### 방법 A — Git clone (Windows PowerShell)
```powershell
git clone https://github.com/jesuswithme/family-journal-page.git "$HOME\.claude\skills\family-journal-page"
```

### 방법 B — 단일 파일 설치 (PowerShell)
```powershell
New-Item -ItemType Directory -Force "$HOME\.claude\skills\family-journal-page" | Out-Null
Invoke-WebRequest "https://raw.githubusercontent.com/jesuswithme/family-journal-page/main/SKILL.md" -OutFile "$HOME\.claude\skills\family-journal-page\SKILL.md"
```

### macOS / Linux
```bash
mkdir -p ~/.claude/skills
git clone https://github.com/jesuswithme/family-journal-page.git ~/.claude/skills/family-journal-page
```

설치 완료 후 Claude Code를 새로 실행하고 스킬을 호출합니다.

## 사용법

사진 3장을 제공한 뒤 다음과 같이 요청합니다.

```text
/family-journal-page
주제: 도아의 탄생으로 행복해진 평화네
인물: 아빠 평화, 엄마 보림, 아기 도아
날짜: 2026.10.18
사진 3장으로 글과 카피를 작성하고 가족 저널 이미지를 만들어 줘.
```

요청 시 날짜·이름·행사 정보가 주어지지 않으면 임의로 지어내지 않습니다.

## 파일
- [SKILL.md](./SKILL.md) — 전체 스킬 지침

## 주의
사진 속 사람의 신원·관계는 사용자 설명이 있을 때만 확인된 것으로 취급합니다. 외부 공개 저장소에 개인 사진이나 이메일 주소를 올리지 않는 것을 권장합니다.
