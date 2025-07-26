---
title: "Session #<% tp.file.title %> – 주제(임시)"
date: <% tp.date.now("YYYY-MM-DD") %>
video_id: ""
duration: ""
tags: [session]
participants: [김하나, A, B]
status: seed  # seed / growing / evergreen
---

## 1. 요점 정리
- …

## 2. 하이라이트

<!-- dv-only:start -->
```dataview
TABLE speaker, timecode, file.link AS 하이라이트
FROM "content/cards"
WHERE type = "highlight" AND session = this.file.name
SORT timecode ASC
```
<!-- dv-only:end -->

## 3. 추천/연관 도서

<!-- dv-only:start -->
```dataview
TABLE title, author, year, file.link AS 도서
FROM "content/cards"
WHERE type = "book" AND contains(mentioned_in, this.file.name)
SORT title ASC
```
<!-- dv-only:end -->

### 추천 도서

### 연관 도서

## 4. 생각해볼 질문

<!-- dv-only:start -->
```dataview
LIST file.link
FROM "content/cards"
WHERE type = "question" AND session = this.file.name
SORT file.name ASC
```
<!-- dv-only:end -->

## 5. 맺음말

<!-- dv-only:start -->
```dataview
LIST file.link
FROM "content/cards"
WHERE type = "message" AND session = this.file.name
```
<!-- dv-only:end -->

<!--
## 6. 전체 타임코드
- 00:00:00 …

## 7. 내부 링크 & 참고
- 관련 테마: [[content/themes/예시]]
- 전사/스크립트: [[content/_transcripts/<% tp.file.title %>]]

---
### 운영 메모
- …
-->