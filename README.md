# da-mockups

DA 팀의 목업·PoC **정적 페이지** 호스팅 레포. GitHub Pages(main 브랜치 루트)로 서빙된다.

```
https://nrise-labs.github.io/da-mockups/<프로젝트>/
```

## 규칙

- **폴더 = 프로젝트.** 각 폴더에 self-contained `index.html` 하나 (외부 의존성 최소화).
- ⚠️ **이 레포와 페이지는 전체 인터넷 공개다.** 미출시 기능 컨셉·에셋을 올릴 때는 노출 판단을 먼저.
  사내 한정이 필요하면 S3 서명 URL(기간 한정)을, 서버가 필요하면(API 키·DB·LLM 프록시)
  Firebase Functions 또는 growth-web 경로를 쓴다. **API 키를 페이지에 넣지 않는다.**
- Framer 반입: Embed 컴포넌트에 페이지 URL을 붙이면 된다 (X-Frame 차단 없음).

## 프로젝트

| 폴더 | 내용 | 소스 |
|---|---|---|
| [`taropo/`](https://nrise-labs.github.io/da-mockups/taropo/) | 타로포 — 세포 데일리 연애운 타로 목업 (리더의 말=템플릿 모드) | athena-query-assistant `JP/scripts/sepo_tarot/` |
