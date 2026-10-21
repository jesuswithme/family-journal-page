---
name: family-journal-page
description: 사진 3장과 주제에서 감성적인 한국어 가족 기록 글과 카피를 작성하고, 원본 사진의 정체성을 유지하는 미니멀 가족 라이프 저널 페이지를 제작한다. 가족 기록, 출생, 기념일, 교회 행사, 감사 일기에 사용.
---

# Family Journal Page — 사진 3장 → 글·카피 → 이미지

## 트리거
사용자가 사진 3장과 주제(또는 상황 설명)를 제시하고 가족 기록 페이지, 사진 저널, 가족 일기, 기념 페이지를 만들고자 할 때 실행한다. `/family-journal-page` 호출도 허용한다.

## 입력
- 필수: 실제 사진 3장, 주제 또는 사진에서 분명히 확인되는 사건
- 선택: 인물 이름과 관계, 날짜, 장소, 강조하고 싶은 신앙·감성 메시지, 이메일/서명, 비율, 분량, 문체, 사진 순서
- 날짜·인물 이름·관계 등 사진만으로 확인할 수 없는 사실을 추정하지 않는다.
- 누락된 필수 정보가 있으면 필요한 것만 간단히 묻는다. 별도 지정이 없으면 세로형 A4에 가까운 5:7 비율, 따뜻하고 담백한 한국어 존댓말/기록체를 기본으로 한다.

## 전체 진행 순서

### 1. 사진 검토
사진마다 장면을 한 문장으로 기록하고 가장 중심이 되는 컷을 정한다. 사람의 신원, 관계, 행사명 등은 사용자가 제공한 정보로만 확정한다. 출생·교회 행사·여행 등 주제와 사진의 연결점을 찾아 기승전결을 구성한다. 개인 정보는 사용자가 포함하도록 지정한 것만 사용한다.

### 2. 카피와 본문 작성
한 번의 응답에서 먼저 아래의 원고를 보여 준다.
- 메인 제목 1개: 감성적이되 구체적인 한국어 15~35자 안팎
- 부제 또는 대표 카피 1개: 1줄
- 사진별 짧은 카피 3개: 각 1줄
- 본문 1개: 5~8개 짧은 문단, 사용자 요청 시 분량을 늘린다.
- 하단 서명 및 날짜: 제공된 값만 기록
사실(이름·연도·성경 구절)을 검토한다. 성경 구절을 직접 인용하면 장절을 정확히 표기하고 확실하지 않으면 인용을 생략한다.

### 3. 이미지용 원고 압축
전체 글을 페이지 하단에 무조건 밀어 넣지 않는다. 3장 사진을 충분히 크게 보이도록 하며 하단에는 **본문 요약 120~250자**를 권장한다. 사용자가 원문 전체 수록을 명시하면 글자 크기를 무리하게 줄이지 말고 2페이지 구성이나 긴 세로 페이지를 제안한다. 원문 전체는 별도 텍스트로 보존한다.

### 4. 디자인 및 이미지 생성
사용 가능한 이미지 편집/생성 기능에 사진 3장과 최종 타이틀·본문을 전달한다.

**사진 원본 보존 최우선**
- 사진을 재그리거나 인물을 재생성하지 말 것. 얼굴·표정·머리·의상·자세·배경 인물의 수를 바꾸지 말 것.
- 가장 확실한 방식은 **실제 원본 사진을 캔버스에 직접 합성하는 편집**이다. 이미지 생성만 이용하면 얼굴과 텍스트가 달라질 수 있으므로 원본 유지가 보장된다고 말하지 않는다.
- 사진은 1장 크게, 2장 작게 자연스럽게 겹치고 부드러운 종이 그림자를 적용한다. 폴라로이드 프레임 금지.
- 크림빛 질감 종이, MUJI/Kinfolk 계열의 미니멀 에디토리얼, 정적인 일상의 따뜻함, 충분한 여백, 손글씨 느낌을 유지한다.
- 제목은 상단 약 15%에 큰 붓글씨, 본문은 아래 약 20~30%에 읽기 쉬운 필기체 혹은 고품질 한글 글꼴, 서명·날짜는 최하단 작은 회색 글자.
- 본문이 길다면 사진을 억지로 줄이지 않고 종이 높이를 늘리거나 페이지를 분리한다.
- 스티커·아이콘·번호표·과장된 콜라주 장식을 피한다.
- 사용자 지정 비율이 있으면 우선한다.

### 5. 검수·결과 제공
- 세 사진이 모두 실제 원본인지, 인물의 얼굴이 변형되지 않았는지 확인한다.
- 제목·이름·날짜·성경 구절·이메일 오탈자를 확인한다.
- 문구가 잘리거나 글자 획이 어긋났다면 텍스트를 재합성한다.
- 결과물은 이미지 1개와 복사 가능한 최종 제목/글/카피로 제공한다.
- 원본 사진 보존이 중요한 경우 이미지 생성 모델이 다시 해석한 결과 대신 원본 파일을 사용한 편집·합성 방식을 우선한다.

## 이미지 생성 지시문 템플릿
Create a premium Korean family life journal page from the **three supplied real photographs**. Keep the source photos as unaltered real photos, never redraw or regenerate people. Place one main photograph large and two smaller photographs with casual, slightly imperfect overlap and natural paper shadows. Use an off-white textured paper background, natural warm lighting, quiet MUJI/Kinfolk editorial mood and generous negative space. No stickers, no illustrated ornaments and no Polaroid borders.

Title in expressive warm-black Korean brush calligraphy near the top: [TITLE]
Short handwritten Korean note with legible spacing: [CONDENSED_BODY]
Footer centered, low contrast: [FOOTER], [DATE]
Use aspect ratio [RATIO]. Keep wording and proper names exact. Do not change the original people's faces, hairstyles, clothes or positions. If exact source-photo retention isn't technically possible, do not falsely claim exact preservation.

## 사용 예
`/family-journal-page 사진 3장 첨부. 주제: 도아의 탄생으로 행복해진 평화네. 이름: 아빠 평화, 엄마 보림, 아기 도아. 날짜: 2026.10.18. 비율 5:7. 제목과 본문 먼저 작성하고 이어서 이미지 제작.`
