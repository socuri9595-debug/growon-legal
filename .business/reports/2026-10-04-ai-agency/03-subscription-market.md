# 03. 시장 심층 분석: 스타트업 AI 자동화 구독 (처리량 정액)

- 작성: 시장 분석가 (3단계 심층) / 작성일·검색일: 2026-10-04
- 대상: 후보 6번. 월 99만원(라이트)·199만원(스탠다드). 자동화·내부툴·AI 기능 요청을 계속 받고, 한 번에 1건씩 48~72시간 안에 납품한다. 1인 운영, 온라인 영업.
- 입력 자료: `founder-profile.md`, `02-ideas.md` 6번, `02-screening.md` 6번, `01-trends.md`, `01-market-landscape.md`
- 환율 가정: 1달러 = 1,400원, 1파운드 = 1.34달러, 1유로 = 1.08달러 (2026-10 기준 실시간 환율은 확인하지 않음)
- 한계: 이번 세션에서는 경쟁사 사이트를 직접 열지 못했다(9dogs.me, getautomated.agency, automatio.io, figue.ai 모두 네트워크에서 차단됨). 해당 업체의 가격은 **검색 결과 요약에 나온 값**이다. 결제 전 원문 확인이 필요하다.

---

## 0. 결론 요약

| 질문 | 판단 |
|---|---|
| 시장이 충분히 큰가 | **1인 사업 기준으로는 충분하다.** 국내 SAM 약 1,000억원/년(추정). 필요한 고객은 4~5곳이 상한이다. 문제는 시장 크기가 아니라 **구독이라는 구매 방식이 국내에서 검증되지 않았다는 점**이다 |
| 돈을 낼 고객이 있는가 | **조건부.** 신입 개발자 1명의 실부담은 월 280만~380만원이다. 이것과 비교하면 199만원은 싸다. 하지만 비교 대상이 크몽 n8n 단건(2만~100만원)이 되는 순간 비싸진다. **월 백로그가 4건 이상인 회사에게만 구독이 합리적이다** |
| 이길 수 있는가 | **국내에서는 "AI 자동화 특화 + 9DOGS보다 싼 가격 + 더 빠른 납기"로 틈이 있다. 해외에서는 가격 우위가 없고 과열돼 있다.** 해자는 약하다. 운영·호스팅을 포함해 만드는 전환 비용이 사실상 유일한 해자다 |
| 국내 vs 해외 | **국내 먼저(0~3개월) → 해외는 3개월 차부터 글 기반 콘텐츠로 병행 실험.** 해외 단가는 1.5~3배 높고 비동기 운영 사례(Designjoy)도 있다. 하지만 레퍼런스 0개인 아시아 1인 공급자에게는 신뢰 장벽과 저가 경쟁(Upwork n8n 공고 중앙값 시간당 $23)이 크다 |
| 12개월 SOM | 국내 **구독 2~4곳(기준 3곳)**, 해외 **0~2곳**. 매출 기준 약 연 0.7억~1.2억원(구독 MRR + 단건 매출) |

---

## 1. 타깃 고객

### 1-1. 모집단 공식 통계 (한국)

| 지표 | 수치 | 기준 | 출처 |
|---|---|---|---|
| 연간 창업기업 수 | 113만 5,561개 (-4.0%) | 2025년 | [중기부 2025 연간 창업기업동향](https://www.korea.kr/briefing/pressReleaseView.do?newsId=156746360&call_from=rsslink) |
| 그중 기술기반 창업 | 22만 1,063개 (+2.9%, 비중 19.5%, 역대 최고) | 2025년 | 같은 자료 |
| 벤처확인기업 | 38,598개사 (벤처투자형 8,296 / 연구개발형 5,319 / 혁신성장형 24,754) | 2025.12 말 | [벤처확인기업 현황](https://www.smes.go.kr/venturein/statistics/viewVentureCurrent), [네이트 뉴스](https://news.nate.com/view/20251228n05242) |
| 벤처기업 평균 매출 | 66.8억원, 총 종사자 82.8만명 | 2024년 실적 | [벤처기업정밀실태조사 보도](https://news.nate.com/view/20251228n05242) |
| 스타트업 투자 건수 | 전체 1,155건 / 6조 5,724억원 | 2025년 | [THE VC](https://thevc.kr/discussions/korea_startup_funding_2025), [와우테일](https://wowtale.net/2026/01/02/252647/) |
| 초기(시드~시리즈A) 투자 | **847건 (-40.4%)**, 1조 9,190억원 (-29.2%) | 2025년 | [THE VC 초기 투자 동향](https://thevc.kr/discussions/korea_startup_funding_25_seed) |
| 시드 투자 중앙값 | 4억원 (2024년 2억원) | 2025년 | 같은 자료 |

해석
- **"투자 받은 시드~A 스타트업"은 연간 약 850곳뿐이고, 1년 사이 40% 줄었다.** 이 집단만 노리면 시장이 좁다. 게다가 투자금은 개발자 채용과 마케팅에 먼저 쓰인다.
- 더 큰 모집단은 **벤처확인기업 3.9만 곳(평균 매출 66.8억원)**이다. 매출이 있는 IT·서비스 중소기업이 여기에 해당한다. 199만원을 낼 능력은 이쪽이 더 확실하다.

### 1-2. 세그먼트별 지불 의향 평가

| 세그먼트 | 월 99만~199만원 지불 능력 | 백로그(월 4건 이상 요청) | 비동기·원격 수용 | 영업 도달(온라인) | 종합 |
|---|---|---|---|---|---|
| **A. 매출 있는 소규모 IT·이커머스·B2B 서비스 회사** (직원 5~30명, 개발자 0~1명, 운영·그로스 담당이 노코드로 버팀) | 높음 (매출 기반, 예산 삭감 위험 낮음) | 높음 (리드·CRM·리포트·CS 분류·정산 등 반복 업무) | 중간~높음 | 중간 (링크드인, 커뮤니티, 지인) | **Beachhead 1순위** |
| B. 시드~프리A 스타트업 (비개발자 창업자 또는 개발자 1~2명이 제품 개발에 묶임) | 중간 (투자금 소진 압박, 2025년 초기 투자 -40%) | 중간~높음 | 높음 (Slack·노션 문화) | 높음 (디스콰이엇·링크드인·AC) | **2순위**. 이탈·폐업 위험이 크다 |
| C. 마케팅·디자인·광고 에이전시 (직원 5~20명) | 중간 | 높음 (고객사 리포트, 대시보드, 소재 자동화) | 높음 | 중간 | 3순위. 화이트라벨(10번)과 겹친다. 레퍼런스가 생긴 뒤 공략 |
| D. 개발자 없는 비IT 중소기업 (제조·유통·전문직) | 높음 | 낮음~중간 (요구사항이 불명확함) | **낮음** (전화·방문 선호, 요구사항 정리에 미팅이 필요) | 낮음 | 비추천. 창업자의 "말하기 어려움, 대면 최소화" 조건과 충돌 |
| E. 1인 창업자·프리랜서 | **낮음** (월 199만원은 매출 대비 과함) | 낮음 | 높음 | 높음 | 비추천. 99만원 라이트도 크몽 단건과 비교당한다 |

### 1-3. Beachhead 정의 (구체)

- **누가**: 직원 5~30명, 연매출 10억~100억원. IT 서비스·SaaS·이커머스·B2B 서비스 회사. 개발자가 없거나 1명이고, 그 1명은 본 제품 개발에 묶여 있다. 구매 결정자는 대표 또는 COO·운영 리드다.
- **어떤 상황에서**: 영업·운영·CS 담당자가 매주 엑셀·구글시트·수작업으로 같은 일을 반복한다. 리드 정리, CRM 입력, 주간 지표 집계, 문의 분류, 계약서·견적서 처리 등이다. "자동화하면 좋겠다"는 목록이 5~20개 쌓여 있지만 개발자 우선순위에서 계속 밀린다.
- **무엇이 불편한가**: ① 개발자를 뽑기에는 일의 양이 애매하다. ② 외주 단건은 매번 견적·계약·검수를 해야 해서 번거롭다. 위시켓 수수료 20~25%도 부담이다. ③ 노코드로 직접 만들면 담당자가 퇴사하는 순간 아무도 관리하지 못한다.
- **지금 어떻게 해결하고 얼마를 쓰나** (추정, 아래 근거)
  - 담당자 시간: 주 5~10시간 × 인건비 → 월 50만~100만원 상당의 기회비용 (가정: 담당자 월 인건비 400만원, 주 40시간 기준)
  - 크몽 n8n 단건: 건당 2만~100만원 ([kmong 723021](https://kmong.com/gig/723021) 2만/5만/15만원, [kmong 716533·721891 등](https://kmong.com/gig/716533) 10만/30만/100만원 패키지)
  - 위시켓 AI·자동화 외주: 건당 30만~450만원 (`01-market-landscape.md`)
  - 노코드 툴 구독: n8n 클라우드 €24~800/월 ([CloudZero](https://www.cloudzero.com/blog/n8n-pricing/)), 그 외 AI 툴 구독(직장인 1인당 월 약 15만원, [머니투데이 2026.01](https://www.mt.co.kr/tech/2026/01/25/2026012310563225007))

### 1-4. 정규 채용과 비용 비교

| 대안 | 월 비용 | 근거 |
|---|---|---|
| 스타트업 신입 개발자 | 연봉 2,800만~3,800만원 → 월 233만~317만원. 4대보험·퇴직금 약 20%를 더하면 **월 280만~380만원 실부담** | [prime-career 2025](https://prime-career.com/article/11240), [ZDNet 2025.10](https://zdnet.co.kr/view/?no=20251031165659) |
| 백엔드 5년차 | 연평균 4,392만원 → 실부담 월 약 440만원 | [prime-career](https://prime-career.com/article/11287) 인용 수치 |
| 신입 전체 평균 | 연 3,243만원 | 같은 자료 |
| 9DOGS 개발자 구독 | 월 250만원 (정가 300만원) | `02-screening.md` |
| **본 서비스 스탠다드** | **월 199만원** (신입 실부담의 52~71%) | — |
| 크몽 단건 n8n (월 3건 가정) | 월 6만~300만원 | 위 크몽 상품 |

**판정**: "개발자 1명 대신"이라는 메시지는 설득력이 있다. 하지만 정직하게 보면, 구매자가 실제로 비교하는 대상은 **"필요할 때 크몽에서 한 건씩 사는 것"**이다. 구독이 이기려면 고객의 **월 요청이 4건 이상**이어야 한다. 그리고 "견적·검수 반복이 사라진다", "운영·유지보수가 포함된다"는 점이 가격 차이를 설명해야 한다. 세일즈 콜에서 첫 질문은 "쌓여 있는 자동화 목록이 몇 개인가"여야 한다.

---

## 2. 경쟁·대체재 분석

### 2-1. 국내 경쟁

| 구분 | 경쟁사 | 가격 | 강점 | 약점 | 판매 실적·후기 |
|---|---|---|---|---|---|
| 직접 (개발 구독) | **9DOGS 개발자 구독** | 월 250만원 (정가 300만원), 요청 무제한, 한 번에 1건 | 디자이너·영상PD·AI모델 구독까지 갖춘 라인업, PM 포함, 일시정지·취소 가능, 4대보험·위약금 없음 | 범용 웹·앱 개발 중심이고 AI 자동화에 특화돼 있지 않음. 평균 납기는 "대부분 2일 이내"라고 하지만 다른 자료에는 5영업일 | 사이트에 스타트업 후기 3건(서비스 출시 성공, 비개발자 협업 용이, 요청 추가 효율). **고객 수·매출 미공개** ([9dogs.me](https://9dogs.me/%EA%B0%9C%EB%B0%9C%EC%9E%90-%EA%B5%AC%EB%8F%85-%EC%84%9C%EB%B9%84%EC%8A%A4/)) |
| 직접 (개발팀 구독) | **그릿지 (소프트스퀘어드)** | 미공개 (상담). "1,500만원 이하로 린 스타트업 초기 환경 구축", 분할 지급 가능 | 시리즈A 15억원 투자 유치, IT 인력 자동 매칭 플랫폼, 정량 운영 리포트, 디노 2024·소프트웨이브 2024 전시 | 팀 단위라 단가가 높고, 제품 개발(MVP) 중심 | 언론 보도 위주. **구독 고객 수 미공개** ([스타트업엔](https://www.startupn.kr/news/articleView.html?idxno=51712), [ZDNet](https://zdnet.co.kr/view/?no=20241016092037), [그릿지 블로그](https://blog.gridge.co.kr/outsourcing_platform_best5/)) |
| 직접 (올인원 구독) | **어니스트패밀리** | 상담 후 안내 | 기획·디자인·개발을 한 팀이 처리 | 가격 불투명, 제품 개발 중심 | 미공개 ([honest-family](https://honest-family.com/blog/2026-%EC%99%B8%EC%A3%BC-%EA%B0%9C%EB%B0%9C-%EC%97%85%EC%B2%B4-%EC%B6%94%EC%B2%9C-best-7-%EC%86%94%EC%A7%81-%EB%B9%84%EA%B5%90)) |
| 간접 (프리랜서 단건) | **크몽 n8n·업무자동화 셀러** | 건당 2만~100만원, 운영 월 2,000원 상품까지 존재. 무상 유지보수 2주 | 가격이 압도적으로 낮음, 리뷰 기반 신뢰, 결제 안전 | 품질 편차, 건마다 새로 커뮤니케이션, 유지보수 공백 | 셀러 다수. **가격 기준점을 낮추는 주범** ([kmong 723021](https://kmong.com/gig/723021), [kmong 736279](https://kmong.com/gig/736279)) |
| 간접 (외주 플랫폼) | **위시켓** | AI·자동화 건당 30만~450만원, 큰 건은 PoC 1,500만~4,000만원 | AI 의뢰 급증(2026 H1 매출 122억원, 2025년 연간 119억원 초과) | 수수료 20~25%, 입찰 경쟁, 매번 견적 | 공개 지표 있음 ([위시켓 블로그](https://blog.wishket.com/blog/wishket-ai-project-growth), [TreeSoop](https://treesoop.com/blog/ai-dev-outsourcing-guide-2026)) |
| 간접 (노코드 자동화 대행) | 각종 노코드 에이전시 | 월정액 10만~100만원 시세 | 저가 월 운영 | 개발 범위가 좁음 | `02-screening.md` ([treesoop](https://treesoop.com/blog/2026-ai-workflow-automation-company-recommendation)) |
| 대체재 | 노코드·AI 직접 사용 (n8n, Zapier Agents, ChatGPT, Lovable, Replit Agent) | 월 $20~수백 | 가장 싸고 즉시 사용 가능. Zapier는 9,000개 이상의 앱 연동, 자연어로 워크플로 생성 | 담당자 시간 소모, 유지 책임, 복잡한 통합에서 막힘 | Lovable은 2026년 8월 시리즈C 4억달러(기업가치 133억달러) 유치 ([tech-insider](https://tech-insider.org/replit-vs-lovable-vs-bolt-new-2026/)) |
| 대체재 | 정규 채용 (신입 개발자) | 월 280만~380만원 실부담 | 전담, 맥락 축적 | 채용 시간, 고정비, 일감이 애매함 | 1-4절 참고 |

### 2-2. 해외 경쟁 (개발 구독·AI 자동화 구독)

| 경쟁사 | 가격 (월) | 원화 환산 | 구조 | 비고·실적 |
|---|---|---|---|---|
| Designjoy (원조, 디자인) | $4,995 | 약 700만원 | 무제한 요청, 1건씩, Trello 비동기, **통화·미팅 없음** | 1인 운영. 2024년 매출 $3.1M, 2025년 6월 MRR $145K. 동시 고객 20~35곳 ([startupfounderstories](https://startupfounderstories.com/stories/brett-williams-designjoy), [dealroom](https://app.dealroom.co/news/note/how-brett-williams-built-a-2m-solo-unlimited-design-subscription-business-with-demand-based-pricing-no-calls-and-productized-add-ons), [Medium](https://medium.com/@zack_liu/the-designjoy-blueprint-how-1-person-handles-35-clients-at-5-000-month-no-meetings-allowed-6fd59df830fe)) |
| Unlimited Dev (영국, 웹 개발) | £995 / £1,895 / £3,195 | 약 187만 / 355만 / 600만원 | 1건씩, 48~72시간 (Pro는 2건 동시, 24~48시간) | **본 서비스와 구조·가격이 거의 같다** ([unlimiteddev.io](https://www.unlimiteddev.io/)) |
| GetAutomated (AI 자동화) | $1,997부터 | 약 280만원 | 무제한 자동화, 정액 | 실적 미확인 ([getautomated.agency](https://www.getautomated.agency/), 검색 요약) |
| Automatio | $3,900 | 약 546만원 | 무제한 요청·수정·프로젝트, 전담 매니저 | 실적 미확인 ([automatio.io](https://www.automatio.io/unlimited-automation-development), 검색 요약) |
| The Automated Agency | $5,000 (Premium) | 약 700만원 | 컨설팅·구현·유지보수 | ([theautomated.agency](https://theautomated.agency/subscriptions/)) |
| AsyncForge (개발) | €2,000 (Light) | 약 302만원 | 이름부터 비동기 | ([figue.ai 목록](https://www.figue.ai/en/blog/best-unlimited-development-subscriptions), 검색 요약) |
| Awesomic (All-in-One) | $2,995 | 약 419만원 | 디자인+개발 | 같은 출처 |
| Graphixa Web Unlimited | $1,299 / $1,899 | 약 182만 / 266만원 | 1건씩, 24~48시간 | Gumroad 판매 ([gumroad](https://graphixa.gumroad.com/l/tier_two)) |
| LearnCode With RK | $499 | 약 70만원 | 1건씩, 약 48시간 | 저가 개인 셀러 ([gumroad](https://learncodewithrk.gumroad.com/l/services)) |
| AI 자동화 리테이너 (일반) | $500~8,000 (관리 수준별: 기본 모니터링 $500~1,200, 액티브 $1,200~2,500, 그로스 $2,500~4,500, 풀 파트너 $4,500~8,000) | — | 리테이너 | ([Digital Agency Network](https://digitalagencynetwork.com/ai-agency-pricing/), [layer3labs](https://www.layer3labs.io/roi/ai-automation-agency-cost)) |
| Upwork n8n 프리랜서 | 공고 중앙값 **시간당 $23**, 상위 10%는 $45 이상. 프로필 호가는 $40~100 | — | 시간제 | 2026-10-01 기준 최근 30일 공고 62건 ([Upwatcher·devsnipe 인용](https://www.upwork.com/hire/n8n-experts/), [gigradar](https://gigradar.io/blog/upwork-hourly-rate)) |

해석
- 해외 개발·자동화 구독의 **주류 가격대는 월 $1,300~5,000**이다. 199만원(약 $1,420)은 해외 기준으로 **최하단**이다.
- 그러나 해외에는 같은 구조의 공급자가 수십 곳 있고, Upwork에는 시간당 $23 수준의 공고가 깔려 있다. 해외에서 "싸다"는 차별화가 되지 않는다. 오히려 "왜 싸지?"라는 품질 의심을 산다.
- **판매 실적이 공개된 사례는 Designjoy(디자인)뿐이다.** 개발·자동화 구독 중 MRR을 공개한 곳은 찾지 못했다. 생산형 서비스 일반 사례로는 Designpop(1년 안에 MRR $8k), Designfly(18개월에 MRR $10k)가 있다([Indie Hackers](https://www.indiehackers.com/post/services/8k-mrr-within-a-year-after-pivoting-to-productized-services-44N8isCYNJf95AVDnefu), [Indie Hackers](https://www.indiehackers.com/post/services/growing-a-productized-service-to-10k-mrr-in-18-months-with-no-audience-or-network-yUW5XGCZXfLJOolfun3e)). 즉 **"$10k MRR까지 12~18개월"이 일반적인 속도**다. 3~6개월 목표에는 빠듯하다.

### 2-3. 빅테크·플랫폼 흡수 위험: **높음**

- Zapier Agents, OpenAI Agent Builder, Claude, ChatGPT 에이전트 기능이 **"단순 자동화(트리거→요약→슬랙 전송)"를 셀프서비스로 만들고 있다.** 비개발자도 2시간 안에 에이전트 워크플로를 만든다는 자료가 있다([zapier blog](https://zapier.com/blog/best-ai-agent-builder/), [lorphic](https://lorphic.com/openai-agents-for-small-business/)).
- Replit Agent 4와 Lovable은 내부툴·랜딩을 1시간 안에 만들게 해 주며, "$3K~15K 에이전시 초안"을 대체한다고 말한다([madebyagents](https://www.madebyagents.com/blog/replit-agent-4-review-for-business-owners)).
- **결론**: "만들어 주기" 자체는 12~24개월 안에 가치가 계속 떨어진다. 살아남는 가치는 **① 여러 시스템을 엮는 통합 ② 돌아가게 유지하는 운영 책임 ③ 무엇을 자동화할지 골라 주는 판단**이다. 상품 설명도 "개발"이 아니라 "자동화 운영 책임"으로 바꿔야 한다.

---

## 3. 포지셔닝

축 선택
- X축: **범용 개발(웹·앱·디자인)** ↔ **업무 자동화·AI 특화**
- Y축: **단건 견적형** ↔ **월 구독형(처리량 정액)**
- 가격과 납기는 칸 안에 표시했다.

| | 범용 개발 (웹·앱·MVP) | 중간 | 업무 자동화·AI 특화 |
|---|---|---|---|
| **월 구독형** | 9DOGS (250만원, 2~5일) / 그릿지 (상담) / 어니스트패밀리 (상담) / 해외: Unlimited Dev (£995~), Awesomic ($2,995) | 해외: AsyncForge (€2,000) | **[본 서비스] 99만/199만원, 48~72시간, 호스팅·운영 포함** / 해외: GetAutomated ($1,997), Automatio ($3,900) / 국내 노코드 대행 (10만~100만원, 범위 좁음) |
| **혼합 (단건+유지보수)** | 위시켓 개발사 | — | 위시켓 AI 의뢰 (30만~450만원) |
| **단건 견적형** | 크몽 웹·앱 개발 | — | 크몽 n8n 셀러 (2만~100만원) / 직접 사용 (Zapier Agents, ChatGPT, Lovable) |

**판단**: 국내 "월 구독 × AI 자동화 특화" 칸에는 **눈에 띄는 공급자가 없다**(이번 검색 기준). 이 칸은 비어 있다. 다만 비어 있는 이유가 "수요가 없어서"일 수도 있다. 해외에서는 같은 칸에 이미 여러 곳이 있다.

차별화 메시지 후보 (국내)
1. "9DOGS보다 51만원 싸고, AI 자동화에 특화돼 있으며, 48~72시간 안에 납품"
2. "개발자 1명 실부담(월 280만원 이상)의 3분의 2 가격, 채용·퇴직 리스크 없음"
3. "만든 자동화의 호스팅·모니터링·장애 대응까지 구독에 포함" (크몽 단건과 구분하는 핵심)

---

## 4. 시장 규모 (TAM / SAM / SOM)

> 이 니치("AI 자동화 개발 구독")만 따로 집계한 리서치 기관 자료는 **국내·해외 모두 없다.** Top-down은 인접 지출 데이터를 쓴 대리 추정이고, Bottom-up이 더 신뢰할 만하다.

### 4-1. 국내

**Top-down (대리 지표)**
- 위시켓 AI 의뢰 매출: 2025년 119억원 → 2026년 상반기 122억원. 연환산하면 **약 244억원 이상**(2026).
- 가정: 위시켓이 국내 중소·스타트업 AI·자동화 외주 지출의 20~30%를 차지한다(크몽, 개발사 직거래, 지인 외주는 제외된 수치이므로).
- 국내 중소·스타트업 AI·자동화 외주 지출 ≈ 244억 ÷ 0.2~0.3 = **약 800억~1,200억원/년** (추정)

**Bottom-up**
| 단계 | 계산식 | 결과 | 가정 |
|---|---|---|---|
| TAM | 대상 기업 6만 곳 × 월 150만원 × 12개월 | **약 1.08조원/년** | 대상 기업 = 벤처확인기업 38,598곳 + 벤처 미확인 IT·이커머스 중소기업 약 2만 곳(추정). 평균 객단가 150만원 = 99만원과 199만원을 반반으로 가정 |
| SAM | 6만 곳 × 10% × 150만원 × 12 | **약 1,080억원/년** | 10% = 개발자가 없거나 과부하 상태 × 월 백로그 4건 이상 × 원격·구독 구매를 받아들임 × 온라인으로 도달 가능. Top-down 대리 추정(800억~1,200억원)과 비슷한 규모 |
| SOM (12개월) | 구독 3곳 × 평균 170만원 × 평균 유지 6개월 + 단건 매출 | **약 3,000만원(구독) + 1,500만~3,000만원(단건) ≈ 연 0.5억~0.6억원 실현 매출**. 12개월 차 MRR 약 500만원 | 1인 상한 4~5곳. 아래 4-3절 |

### 4-2. 해외 (미국 중심, 글로벌 영어권)

**Top-down**: 니치 시장 규모 자료 없음. 대신 가격대 근거만 확보했다. 자동화 리테이너 월 $500~8,000, 개발 구독 월 $1,300~5,000 (2-2절).

**Bottom-up**
| 단계 | 계산식 | 결과 | 가정 |
|---|---|---|---|
| 모집단 | 미국 고용주 기업 6,395,635곳 | — | [SBA 2025 Profile](https://advocacy.sba.gov/wp-content/uploads/2025/06/United_States_2025-State-Profile.pdf). 참고로 2025년 미국 사전 시드 SAFE·전환사채 50,316건, priced seed 약 1,494건 ([Carta](https://carta.com/data/state-of-pre-seed-2025/)) |
| TAM | 30만 곳 × $1,500 × 12 | **약 $5.4B/년 (약 7.6조원)** | 30만 곳 = 고용주 기업의 약 5%(디지털 운영 비중이 높고 월 $1,500 이상의 자동화 예산이 가능한 곳, 추정). 영국·캐나다·호주를 더하면 더 커짐 |
| SAM | 30만 × 5% × $1,500 × 12 | **약 $270M/년 (약 3,780억원)** | 5% = 해외 1인 공급자에게 비동기로 맡길 의향 × 글 기반 채널로 도달 가능 |
| SOM (12개월) | 0~2곳 × $1,500~2,000 × 평균 4개월 | **$0~16,000 (0~2,200만원)** | 첫 계약은 3개월 차 콘텐츠 시작 후 빨라야 4~6개월 차. Indie Hackers 사례상 $10k MRR까지 12~18개월 |

### 4-3. 12개월 현실적 고객 수 (시나리오)

| 시나리오 | 국내 구독 (12개월 차 유지) | 해외 구독 | 단건 프로젝트 (누적) | 12개월 차 MRR | 조건 |
|---|---|---|---|---|---|
| 비관 | 0~1곳 | 0곳 | 5~8건 | 0~199만원 | 국내 구매자가 "단건 견적"만 원함 → 위시켓·크몽 단건 외주로 전락 (`02-screening` Kill 기준) |
| **기준** | **2~3곳** (누적 계약 5~6곳, 2~3개월 차 이탈 감안) | 0~1곳 | 8~12건 | **약 400만~700만원** | 단건 → 구독 전환율 25~30%, 월 이탈률 10~15% (B2B 이탈의 43%가 첫 90일에 발생, [duet.so](https://duet.so/blog/turn-ai-agent-builds-into-recurring-retainers)) |
| 낙관 | 4곳 (1인 상한) | 1~2곳 ($1,995) | 10건 이상 | 약 1,000만~1,100만원 | 빌드 인 퍼블릭 콘텐츠가 인바운드를 만들고, AC 제휴 1곳 확보 |

**주의**: 기준 시나리오에서도 3~6개월 안에 월 500만원은 "가능하지만 보장되지 않음" 수준이다. 이탈 1곳이 MRR의 25~33%다.

---

## 5. 해외(영어 글 기반) 원격 판매 가능성

| 항목 | 판단 | 근거 |
|---|---|---|
| 가격 수준 | **해외가 1.5~3배 높다.** 같은 구조의 Unlimited Dev가 £995(약 187만원)부터, AI 자동화 구독은 $1,997~5,000 | 2-2절 |
| 비동기(글)만으로 운영 | **가능하다. 사례가 있다.** Designjoy는 통화·미팅 없이 Trello로만 운영하고, 판매 콜도 없애 랜딩에서 바로 결제받는다. AsyncForge처럼 비동기를 브랜드로 내세운 개발 구독도 있다 | [dealroom](https://app.dealroom.co/news/note/how-brett-williams-built-a-2m-solo-unlimited-design-subscription-business-with-demand-based-pricing-no-calls-and-productized-add-ons), [assembly.com](https://assembly.com/blog/productized-services) |
| 반대 근거 | 해외 오프쇼어 협업 가이드는 하루 3~4시간의 시간대 겹침과 결정 시점의 동기 미팅을 권장한다. 비원어민 프리랜서에게 "화상통화 가능한 업무 수준 영어"를 요구하는 자료도 있다. 한국-미국 동부는 13~14시간 차이라 겹치는 시간이 거의 없다 | [outsourceaccelerator](https://www.outsourceaccelerator.com/articles/hire-offshore-developers-startups/), [assembly.com](https://assembly.com/blog/productized-services) |
| 결제 | **Stripe는 한국 사업자를 직접 지원하지 않는다.** 대안은 Gumroad(한국 은행 계좌 직접 정산, 최소 4만원, 수수료 약 10%), PayPal, Wise 인보이스, 또는 Stripe Atlas로 미국 법인 설립($500) | [OneSafe](https://www.onesafe.io/blog/does-stripe-work-in-korea), [Gumroad](https://gumroad.gumroad.com/p/local-bank-account-support-in-more-countries) |
| 신뢰 장벽 | 레퍼런스 0개, 해외 결제 이력 없음, 아시아 1인 공급자 → 데이터·보안 접근 권한을 받기 어렵다. 저가 공급자(인도·동남아·동유럽)와 같은 범주로 묶인다 | 추정 |
| 세무 | 한국 개인사업자로 영세율 용역 수출 신고가 가능하다(세무사 확인 필요) | [solarstaff](https://help.solarstaff.com/en/articles/9736740-freelance-and-taxes-south-korea) |

**판정**: 해외는 **"가격은 높지만 고객 확보가 느린 시장"**이다. 비동기 운영 자체는 문제가 되지 않는다. 문제는 신뢰와 유입이다. 콜드 아웃리치(통화 없이 메일·DM)로 시작하면 저가 경쟁에 묻힌다. 따라서 **국내에서 사례 2~3개를 만든 뒤, 3개월 차부터 영어 빌드 인 퍼블릭(X, 링크드인, Indie Hackers)과 Gumroad 결제 랜딩을 붙이는 순서**가 맞다. 해외 가격은 $1,495(라이트)~$2,495(스탠다드)로 국내보다 높게 잡는다. 국내 가격을 그대로 쓰면 저가로 보인다.

---

## 6. 진입 장벽·해자

| 해자 유형 | 가능성 | 설명 |
|---|---|---|
| 데이터 | 낮음 | 고객사 데이터는 고객 것이다. 다만 "업종별 자동화 템플릿·프롬프트 라이브러리"가 쌓이면 납기 단축(원가 우위)으로 이어진다 |
| 네트워크 효과 | 없음 | — |
| **전환 비용** | **중간 (가장 현실적)** | 만든 자동화의 호스팅(n8n·Supabase), 모니터링, API 키 관리를 구독에 포함하면, 해지할 때 이전 작업이 필요해진다. 단, 고객에게 불리한 락인으로 보이면 신뢰를 잃는다. "해지 시 이관 패키지를 유료로 제공"하는 식으로 공정하게 설계한다 |
| 유통 채널 | 낮음~중간 | AC·창업지원기관 제휴(포트폴리오사 혜택)를 확보하면 반복 유입 채널이 된다. 빌드 인 퍼블릭 콘텐츠는 6개월 이상 쌓여야 자산이 된다 |
| 도메인 전문성 | 중간 | 특정 업종(이커머스 운영, B2B SaaS 세일즈옵스)에 집중하면 "그 업종의 자동화 목록"을 먼저 제안할 수 있다. 범용으로 가면 해자가 없다 |
| 진입 장벽 (경쟁자 입장) | **매우 낮음** | Claude Code·n8n을 다룰 줄 아는 사람은 누구나 오늘 같은 랜딩을 열 수 있다. 해외에서는 이미 그렇게 됐다 |

**결론**: 해자는 약하다. 이 사업은 "방어 가능한 회사"가 아니라 **"현금흐름을 만드는 1인 서비스"**로 봐야 한다. 그 목적(3~6개월 현금흐름)에는 맞는다.

---

## 7. 온라인 유입 채널과 정보통신망법 50조

### 7-1. 채널별 평가

| 채널 | 대상 | 방식 | 기대 효과 | 리스크·메모 |
|---|---|---|---|---|
| **지인 창업자·IT 업계 1:1 연락** | A·B | 개인적으로 아는 사람에게 개별 메시지 | 첫 1~2곳의 가장 빠른 경로 | 지인이라도 영리 광고 메시지는 50조 대상이 될 수 있다. 먼저 "의견을 묻는" 형태로 시작해 동의를 받는다 |
| **링크드인 (국문·영문)** | A·B·해외 | 빌드 인 퍼블릭: "이번 주 만든 자동화 + 절감 시간" 게시. DM은 상대가 먼저 반응한 경우에만 | 중간. 3개월 이상 지속해야 효과 | 일방적인 영업 DM은 50조 위험(7-2절) |
| **X build-in-public (영문)** | 해외·B | 짧은 데모 영상·스레드 | 해외 인바운드의 핵심 채널 | 효과까지 3~6개월 |
| **디스콰이엇** | B | 메이커 로그, 프로덕트 등록 | 중간 | 2025년 10월 릴레잇(픽셀릭)에 인수됐다. THE VC에는 법인 폐업(2025.12)으로 표시된다. 서비스는 이어지지만 **커뮤니티 활력은 확인이 필요**하다 ([머니투데이](https://www.mt.co.kr/future/2025/10/30/2025103010105511832), [THE VC](https://thevc.kr/disquiet)) |
| **GeekNews (Show GN)** | 개발자·창업자 | 직접 만든 오픈소스·도구 소개(마케팅 문구 금지 규칙) | 신뢰 형성에 좋음 | 서비스 홍보 글은 규칙 위반. **무료 템플릿·오픈소스를 공개**하는 방식으로만 활용 ([hada.io](https://hada.io/blog/geeknews-show/)) |
| **위시켓 입찰** | A·B | AI·자동화 프로젝트 입찰 | 단건 매출 + 고객 접점 | 수수료 20~25%. 플랫폼 밖 직거래 전환 제한 정책 확인 필요 |
| **크몽·크몽Biz** | A·E | "자동화 진단 + 1건 구축" 입구 상품 | 인바운드 | 저가 경쟁. 구독 전환 시 플랫폼 정책 확인 |
| **AC·창업지원기관 제휴** | B | "포트폴리오사 첫 달 50%" 혜택으로 제휴 등록, 오피스아워·웨비나(글·화면공유 중심) | 높음 (기관이 자기 채널로 공지하므로 50조 위험이 낮음) | 제휴까지 시간이 걸린다. 공급기업 등록형 바우처(혁신바우처 등)는 프로젝트형이라 구독과 맞지 않는다 ([혁신바우처 2026 공고](https://www.bizinfo.go.kr/web/lay1/bbs/S1T122C128/AS/74/view.do?pblancId=PBLN_000000000116305)) |
| 스타트업 오픈채팅·슬랙 커뮤니티 | B | 정보성 글(자동화 사례) + 무료 데모 신청 폼 | 중간 | 방마다 홍보 규칙이 다르므로 운영자 허락을 먼저 받는다 |
| 영문 Indie Hackers·Reddit (r/SaaS 등) | 해외 | 사례 글 | 낮음~중간 | 직접 홍보 금지 규칙이 많음 |

### 7-2. 정보통신망법 제50조 회피(준수) 방법

**법 요지**: 전자적 전송매체(이메일, 문자, 메신저 등)로 **영리 목적의 광고성 정보**를 보내려면 **수신자의 명시적 사전 동의**가 필요하다. 주된 내용이 광고가 아니어도 광고가 부수적으로 섞이면 전체가 광고성 정보로 본다. 위반 시 과태료는 3,000만원 이하다. 예외는 **거래관계를 통해 수신자에게서 직접 연락처를 받은 경우, 거래 종료 후 6개월 이내의 동종 재화·용역 광고**뿐이다. 명함처럼 서면으로 연락처를 받은 경우 거래관계 예외가 적용될 여지가 있다는 해석이 있다. **공개된 이메일에 대한 명시적 예외 규정은 확인하지 못했다.** ([CaseNote 법제처 해석](https://casenote.kr/%EB%B2%95%EC%A0%9C%EC%B2%98/24-0311-a473be), [디지털데일리 스타트업 법률상식](https://m.ddaily.co.kr/page/view/2021090610521515261), [KISA 안내서](https://www.postplus.co.kr/images/%EC%A0%95%EB%B3%B4%ED%86%B5%EC%8B%A0%EB%A7%9D%EB%B2%95_%EC%95%88%EB%82%B4%EC%84%9C.pdf))

**실행 원칙** (법률 자문 전 보수적 운영안)
1. **인바운드 우선**: 콘텐츠(빌드 인 퍼블릭, 무료 템플릿)를 보고 상대가 먼저 연락하게 만든다. 상대가 먼저 문의한 건에 대한 답장은 광고성 정보 전송이 아니다(일반적 해석).
2. **동의 수집 장치**: 랜딩·무료 데모 신청 폼에 "서비스 안내 메일 수신 동의" 체크박스를 별도로 둔다. 동의 일시와 방법을 기록해 보관한다.
3. **공개 요청에 응답**: 위시켓 입찰, 커뮤니티의 "자동화 개발자 구합니다" 글에 대한 댓글·지원은 상대의 공개 요청에 대한 응답이다. 광고 전송보다 위험이 낮다(추정, 플랫폼 규칙은 따로 지킨다).
4. **제3자 채널 활용**: AC·지원기관이 자기 구성원에게 공지하게 한다(그 기관이 자체 수신 동의를 근거로 보냄).
5. **거래관계 예외 활용**: 단건 고객에게는 거래 종료 후 6개월 이내에 구독(동종 용역)을 제안할 수 있다. 단건 → 구독 전환 전략과 법적으로 맞물린다.
6. **부득이하게 개별 제안을 보낼 때**: 제목 앞 "(광고)" 표기, 전송자 명칭·연락처, 수신거부 방법을 반드시 넣는다. **단, 표기 의무를 지켜도 사전 동의가 없다는 위반이 사라지지는 않는다.** 대량 발송은 금지하고, 소수의 맞춤 제안도 법률 자문을 받은 뒤에만 한다.
7. **링크드인 DM**: 메신저 형태도 전자적 전송매체로 볼 여지가 크다. 연결 수락만으로 광고 수신에 동의했다고 보기 어렵다(추정). "의견 질문 → 상대가 관심 표명 → 그다음 안내" 순서를 지킨다.
8. **해외 수신자**: 미국 CAN-SPAM은 옵트아웃 방식이라 수신거부 링크와 실제 주소를 넣으면 B2B 콜드메일이 허용된다. 하지만 **한국에서 보내는 전송에 50조가 적용되는지는 확인이 필요**하다. 결론이 나기 전까지 해외도 인바운드·콘텐츠 중심으로 운영한다.

---

## 8. 분석가 의견: 불리한 근거

- **수요 미검증이 가장 큰 문제다.** 국내 개발 구독 3곳(9DOGS, 그릿지, 어니스트패밀리) 중 고객 수나 매출을 공개한 곳은 없다. 9DOGS 사이트 후기는 3건뿐이다. "공급자가 있다 = 시장이 있다"로 보기 어렵다.
- **초기 스타트업 지갑이 줄었다.** 2025년 시드~A 투자 건수는 40.4% 감소했다. 시드를 받은 회사가 2년 안에 시리즈A로 가는 비율은 미국 기준 15.4%다([Carta](https://carta.com/data/linkedin-seed-to-series-a-still-uphill-battle/)). 스타트업 고객은 폐업·예산 삭감 이탈이 잦다.
- **가격 기준점이 무너지는 중이다.** 크몽 n8n 상품은 2만원부터, Upwork 공고 중앙값은 시간당 $23이다. 단순 자동화는 Zapier Agents·ChatGPT로 직접 만드는 쪽으로 넘어가고 있다.
- **해외는 과열됐다.** 같은 구조와 가격(£995~$2,000)의 공급자가 이미 여럿 있다.
- **유리한 근거**: 국내 "구독 × AI 자동화 특화" 칸은 비어 있다. 199만원은 9DOGS(250만원)와 신입 개발자 실부담(280만원 이상)보다 낮다. Designjoy가 증명했듯 비동기 1인 구독은 운영상 가능하고, 창업자의 "말하기 어려움" 약점을 구조적으로 피할 수 있다.

---

## 출처 (검색일 2026-10-04)

- 통계: [중기부 2025 연간 창업기업동향](https://www.korea.kr/briefing/pressReleaseView.do?newsId=156746360&call_from=rsslink) / [벤처확인기업 현황](https://www.smes.go.kr/venturein/statistics/viewVentureCurrent) / [벤처기업정밀실태조사 보도(네이트)](https://news.nate.com/view/20251228n05242) / [THE VC 2025 투자 통계](https://thevc.kr/discussions/korea_startup_funding_2025) / [THE VC 초기 투자](https://thevc.kr/discussions/korea_startup_funding_25_seed) / [와우테일](https://wowtale.net/2026/01/02/252647/) / [SBA 2025 US Profile](https://advocacy.sba.gov/wp-content/uploads/2025/06/United_States_2025-State-Profile.pdf) / [Carta Pre-Seed 2025](https://carta.com/data/state-of-pre-seed-2025/) / [Carta seed→A](https://carta.com/data/linkedin-seed-to-series-a-still-uphill-battle/)
- 연봉: [prime-career 신입 백엔드](https://prime-career.com/article/11240) / [prime-career 백엔드](https://prime-career.com/article/11287) / [ZDNet 개발자 연봉](https://zdnet.co.kr/view/?no=20251031165659)
- 국내 경쟁: [9DOGS 개발자 구독](https://9dogs.me/%EA%B0%9C%EB%B0%9C%EC%9E%90-%EA%B5%AC%EB%8F%85-%EC%84%9C%EB%B9%84%EC%8A%A4/) / [그릿지 스타트업엔](https://www.startupn.kr/news/articleView.html?idxno=51712) / [그릿지 ZDNet](https://zdnet.co.kr/view/?no=20241016092037) / [그릿지 블로그](https://blog.gridge.co.kr/outsourcing_platform_best5/) / [어니스트패밀리](https://honest-family.com/blog/2026-%EC%99%B8%EC%A3%BC-%EA%B0%9C%EB%B0%9C-%EC%97%85%EC%B2%B4-%EC%B6%94%EC%B2%9C-best-7-%EC%86%94%EC%A7%81-%EB%B9%84%EA%B5%90) / [크몽 723021](https://kmong.com/gig/723021) / [크몽 716533](https://kmong.com/gig/716533) / [크몽 736279](https://kmong.com/gig/736279) / [위시켓 AI 성장](https://blog.wishket.com/blog/wishket-ai-project-growth) / [위시켓 외주 비용](https://blog.wishket.com/blog/outsourcing-development-cost) / [TreeSoop AI 외주 비용](https://treesoop.com/blog/ai-dev-outsourcing-guide-2026)
- 해외 경쟁: [Unlimited Dev](https://www.unlimiteddev.io/) / [GetAutomated](https://www.getautomated.agency/) / [Automatio](https://www.automatio.io/unlimited-automation-development) / [The Automated Agency](https://theautomated.agency/subscriptions/) / [figue.ai 개발 구독 목록](https://www.figue.ai/en/blog/best-unlimited-development-subscriptions) / [Graphixa](https://graphixa.gumroad.com/l/tier_two) / [LearnCode RK](https://learncodewithrk.gumroad.com/l/services) / [Digital Agency Network](https://digitalagencynetwork.com/ai-agency-pricing/) / [layer3labs](https://www.layer3labs.io/roi/ai-automation-agency-cost) / [Upwork n8n](https://www.upwork.com/hire/n8n-experts/) / [gigradar](https://gigradar.io/blog/upwork-hourly-rate)
- Designjoy·생산형 서비스: [startupfounderstories](https://startupfounderstories.com/stories/brett-williams-designjoy) / [dealroom](https://app.dealroom.co/news/note/how-brett-williams-built-a-2m-solo-unlimited-design-subscription-business-with-demand-based-pricing-no-calls-and-productized-add-ons) / [Medium](https://medium.com/@zack_liu/the-designjoy-blueprint-how-1-person-handles-35-clients-at-5-000-month-no-meetings-allowed-6fd59df830fe) / [Indie Hackers Designpop](https://www.indiehackers.com/post/services/8k-mrr-within-a-year-after-pivoting-to-productized-services-44N8isCYNJf95AVDnefu) / [Indie Hackers Designfly](https://www.indiehackers.com/post/services/growing-a-productized-service-to-10k-mrr-in-18-months-with-no-audience-or-network-yUW5XGCZXfLJOolfun3e) / [assembly.com](https://assembly.com/blog/productized-services) / [duet.so 리테이너 이탈](https://duet.so/blog/turn-ai-agent-builds-into-recurring-retainers)
- 빅테크·대체재: [Zapier AI agent builder](https://zapier.com/blog/best-ai-agent-builder/) / [lorphic](https://lorphic.com/openai-agents-for-small-business/) / [tech-insider Lovable](https://tech-insider.org/replit-vs-lovable-vs-bolt-new-2026/) / [madebyagents Replit Agent 4](https://www.madebyagents.com/blog/replit-agent-4-review-for-business-owners) / [CloudZero n8n](https://www.cloudzero.com/blog/n8n-pricing/) / [머니투데이 AI 구독료](https://www.mt.co.kr/tech/2026/01/25/2026012310563225007)
- 해외 판매 인프라: [OneSafe Stripe Korea](https://www.onesafe.io/blog/does-stripe-work-in-korea) / [Gumroad 한국 계좌](https://gumroad.gumroad.com/p/local-bank-account-support-in-more-countries) / [outsourceaccelerator](https://www.outsourceaccelerator.com/articles/hire-offshore-developers-startups/) / [solarstaff](https://help.solarstaff.com/en/articles/9736740-freelance-and-taxes-south-korea)
- 채널·법률: [디스콰이엇 인수 머니투데이](https://www.mt.co.kr/future/2025/10/30/2025103010105511832) / [THE VC 디스콰이엇](https://thevc.kr/disquiet) / [GeekNews Show](https://hada.io/blog/geeknews-show/) / [혁신바우처 2026](https://www.bizinfo.go.kr/web/lay1/bbs/S1T122C128/AS/74/view.do?pblancId=PBLN_000000000116305) / [법제처 해석 CaseNote](https://casenote.kr/%EB%B2%95%EC%A0%9C%EC%B2%98/24-0311-a473be) / [디지털데일리](https://m.ddaily.co.kr/page/view/2021090610521515261) / [KISA 정보통신망법 안내서](https://www.postplus.co.kr/images/%EC%A0%95%EB%B3%B4%ED%86%B5%EC%8B%A0%EB%A7%9D%EB%B2%95_%EC%95%88%EB%82%B4%EC%84%9C.pdf)
