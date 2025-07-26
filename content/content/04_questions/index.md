# 생각해볼 질문


```dataview
TABLE session, audience, file.link AS 질문
FROM "content/cards"
WHERE type = "question"
SORT session DESC
