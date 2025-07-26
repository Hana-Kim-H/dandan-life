---
type: question
session: <% tp.file.title %>
origin: "[[sessions/<% tp.file.title %>]]"
tags: []
---
## 생각해볼 질문

<%*
const content = await app.vault.read(app.workspace.getActiveFile());
const block = content.match(/## 생각해볼 질문([\s\S]*?)(\n## |\n$)/);
tR += block ? block[1].trim() : "질문을 찾을 수 없습니다.";
%>