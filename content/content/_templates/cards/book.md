---
type: book
title: "<% tp.system.prompt('책 제목?') %>"
author: "<% tp.system.prompt('저자?') %>"
year: "<% tp.system.prompt('출간 연도?') %>"
session: "<% tp.system.prompt('언급된 세션(쉼표로 구분 가능)') %>"
why: "<% tp.system.prompt('한 줄 이유') %>"
tags: [book, 추천도서]
---

## 책 정보  
- **제목:** <% tp.frontmatter.title %>
- **저자:** <% tp.frontmatter.author %>
- **출간 연도:** <% tp.frontmatter.year %>

---

## 한 줄 이유  
<% tp.frontmatter.why %>

---

## 관련 키워드  
- [[content/02_themes/예시]]
