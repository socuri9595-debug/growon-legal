# 01. AI 트렌드 조사 — 1인·저예산·초고속 개발자를 위한 기회 지도

- 작성: trend-scout / 작성일: 2026-10-04 / 검색일: 2026-10-04
- 기준 프로필: `.business/founder-profile.md` (1인, Claude Code로 앱 10개 출시, 주 30시간+, 예산 100만원 이하, 한국 기반, 분야 제한 없음)
- 필터: "광고비 없이, 혼자, 몇 주 안에 MVP"로 공략 가능한가를 우선 기준으로 삼음
- 신뢰도 표기: [1차] 공식기관·원 보고서 / [2차] 언론·리서치 요약 / [블로그] 개인·업체 블로그(수치 교차검증 필요) / **추정** = 출처 없는 판단
- 한계: sensortower.com, menlovc.com, fnnews.com, medium.com 등은 이 환경에서 원문 열람이 차단되어 검색 결과 요약으로 확인함. 핵심 수치는 2단계에서 원문을 다시 확인할 것을 권장.

---

## 요약 (한눈에)

| # | 트렌드 | 창업자 적합도 | 타이밍 |
|---|---|---|---|
| 1 | 소비자 AI 앱 매출 폭증, 그러나 리텐션 위기 | 높음 (앱 출시 경험) | 지금 |
| 2 | 해외 1인·소규모 AI 앱의 검증된 매출 (타임머신 후보) | 높음 | 지금 |
| 3 | API 단가 붕괴 + Apple 무료 온디바이스/PCC 추론 | 매우 높음 (iOS 개발자) | iOS 27 출시 직후 = 지금 |
| 4 | 실시간 음성 AI 단가 하락 → AI 전화응대 | 중간 (국내 대기업·정부 경쟁) | 경쟁 심화 중 |
| 5 | 영상 생성 단가 하락 → AI UGC 광고 | 중간~높음 | 지금 |
| 6 | 에이전트 유통 채널(ChatGPT 플러그인, 카카오 PlayMCP) 개방 | 높음 | 초기 선점 구간 |
| 7 | 네이버 AI 브리핑 확대 → GEO 수요 | 높음 | 시장 형성 초기 |
| 8 | AI 기본법 시행 (표시·고지 의무, 계도기간) | 높음 | 계도기간 종료(2027 초) 전 |
| 9 | 정부 AI 지원사업 대규모 편성 | 중간~높음 | 2027 공고 대비 |
| 10 | 국내 AI 투자 쏠림 | 참고 | — |

---

## 트렌드 1. 소비자 AI 앱 매출 폭증 — 그러나 "AI 앱은 빨리 해지된다"

**근거**
- 2025년 글로벌 앱 지출 1,670억 달러, 비게임 앱 인앱결제가 처음으로 게임을 추월(+21% YoY). 생성형 AI 앱 다운로드 38억 건(2배), IAP 매출 50억 달러 이상(약 3배). [2차] Sensor Tower State of Mobile 2026 — https://sensortower.com/press/press-release-boosted-by-gen-ai-services-consumers-spent-more-money-in-apps-than-games-for-first-time (2026 초)
- 생성형 AI 앱 매출: 2023 Q1 6천만 달러 미만 → 2026 Q1 19억 달러(3년간 32배). 2025 Q2~2026 Q1 +232% YoY. 성장 하위 카테고리는 유틸리티, 멀티미디어·디자인, 비즈니스·생산성. 2026년 생성형 AI 앱 소비자 지출 100억 달러 이상 전망, IAP 매출 기준 3위 카테고리로 상승 전망. [2차] Sensor Tower State of AI 2026 — https://www.prnewswire.com/news-releases/sensor-tower-state-of-ai-2026-report-global-time-spent-on-generative-ai-apps-projected-to-more-than-double-year-over-year-302800975.html
- 2026년 글로벌 소비자 AI 지출 400억 달러(전년 120억 달러의 3배 이상), AI 이용자 55%가 1개 이상 유료 결제. [2차] Menlo Ventures, The State of Consumer AI 2026 — https://menlovc.com/perspective/2026-the-state-of-consumer-ai/
- **리텐션 역설**: AI 앱은 결제자당 매출 +41%, 체험→유료 전환율 8.5%(비AI 5.6%)로 높지만, 12개월 리텐션 21.1%(비AI 30.7%)로 30% 더 빨리 해지된다. 월간 신규 구독 앱 출시 수 2022.1 약 2,000개 → 2026.1 14,700개 이상. 2020년 이전 출시 앱이 구독 매출의 69%. [1차] RevenueCat State of Subscription Apps 2026 — https://www.revenuecat.com/state-of-subscription-apps / [2차] TechCrunch 2026-03-10 — https://techcrunch.com/2026/03/10/ai-powered-apps-struggle-with-long-term-retention-new-report-shows
- 한국: 생성형 AI 이용자 24%가 유료 구독, 20대 30.1%. [2차] 서울경제 — https://www.sedaily.com/article/20049653 / 2026.1.1~6.5 한국 iOS 생성형 AI 앱 매출 성장 1위는 Claude, 매출 2위(1위 ChatGPT). Claude 전체 매출 중 한국 비중 4.7%로 미국 다음. [2차] 헤럴드경제 — https://biz.heraldcorp.com/article/10771050 / 한국의 ChatGPT 유료결제는 세계 2위, AI 사용률은 12위라는 보도 [2차, 기사 제목 기준] 파이낸셜뉴스 2026-09-28 — https://www.fnnews.com/news/202609281339387227

**왜 지금인가**
- 소비자가 AI에 돈을 내는 습관이 생겼다(전환율이 높다). 하지만 "챗봇에 껍데기만 씌운 앱"은 금방 해지된다. 기록·습관·데이터가 쌓이는 앱이 이기는 구조다.
- 한국은 결제 의향이 높은데(유료 구독 24%, ChatGPT 유료 세계 2위) 한국어·한국 생활에 맞춘 버티컬 AI 앱은 아직 적다(**추정**).

**파생 기회**
1. 기존 그로우온(목표 시각화) 등 보유 앱 10개에 AI 기능 추가 → 이미 쌓인 사용자 데이터 덕분에 리텐션 약점을 피함.
2. "AI + 기록/습관" 형태의 한국형 버티컬 앱(식단, 공부, 육아, 반려동물, 피부 등). 사진 입력 → 자동 기록 → 주간 리포트.
3. 해지를 막는 장치(누적 데이터, 스트릭, 연간 플랜)를 처음부터 설계한 구독 앱.

---

## 트렌드 2. 해외 1인·소규모 AI 앱의 검증된 매출 (타임머신 후보)

**근거**
- Cal AI(사진으로 칼로리 계산): 고등학생 2명이 창업, 6개월 만에 MRR 100만 달러, 18개월 만에 다운로드 1,500만+, ARR 약 4,000만 달러. 2026년 3월 MyFitnessPal이 인수. [2차] CNBC 2025-09-06 — https://www.cnbc.com/2025/09/06/cal-ai-how-a-teenage-ceo-built-a-fast-growing-calorie-tracking-app.html / [블로그] Latka — https://getlatka.com/companies/calai.app / Superwall 사례 — https://superwall.com/case-studies/cal-ai
- TrackAI(1인 개발 사진 칼로리 앱): 2026-08-30 RevenueCat 기준 활성 구독 5,134개, MRR 20,809달러. [블로그] https://www.sofarbot.com/stories/trackai-oleksandr-yashchuk-20913-verified-mrr
- Pieter Levels Photo AI(1인) MRR 13.2만 달러, 전체 포트폴리오 ARR 300만 달러 이상(직원 0명). [블로그] https://www.buildmvpfast.com/blog/solo-developer-35-micro-saas-apps-77k-month-portfolio-2026 , https://crazyburst.com/ai-saas-solo-founder-success-stories-2026/
- 1인 개발자가 마이크로 SaaS 35개로 월 7.7만 달러를 버는 포트폴리오 사례. [블로그] https://www.buildmvpfast.com/blog/solo-developer-35-micro-saas-apps-77k-month-portfolio-2026
- Base44(1인 창업 AI 앱 빌더)가 6개월 만에 Wix에 8,000만 달러 현금 매각. [블로그] https://superframeworks.com/articles/best-micro-saas-ideas-solopreneurs
- TrustMRR: Stripe 연동으로 매출이 검증된 스타트업 4,075개 목록. AI 카테고리에서 1인·소규모 팀의 월 5천~10만 달러대 사례 다수. [1차] https://trustmrr.com/category/ai
- 인디해커 매출 분포(대략): 50%는 MRR 0~1천 달러, 20%는 1천~1만 달러, 10%는 1만~10만 달러. [블로그] https://www.quvir.com/2026/05/indie-hackers-are-building-10kmonth-ai.html
- 돈이 되는 니치는 "지루하지만 고통이 큰 영역"(결제 실패 복구, 컴플라이언스 서류, 도구 사이를 잇는 워크플로)이라는 관찰. [블로그] https://www.flowjam.com/blog/indie-hackers-saas-ideas-2025-10-you-can-launch-fast
- (주의) "수익을 내는 SaaS의 44%가 1인 운영(Stripe 데이터)"이라는 수치가 돌지만, Stripe 원문은 확인하지 못함 → **미검증**.

**왜 지금인가**
- "사진 한 장 → AI 분석 → 구독" 구조의 앱이 1인 개발로도 월 수천만 원 매출을 낸다는 것이 2025~2026년에 여러 번 확인됐다.
- 한국어·한국 음식·한국 생활에 맞춘 대응은 약하다. 예를 들어 Cal AI 계열 앱은 한식(찌개, 반찬, 공유 접시) 인식과 한국식 1인분 기준에서 약할 가능성이 높다(**추정**, 2단계에서 경쟁 앱 리뷰로 확인 필요).

**파생 기회**
1. 한식에 특화된 사진 칼로리·영양 앱(공유 반찬 분할, 편의점 제품 DB, 배달 메뉴 인식).
2. 한국형 "사진 → 진단" 버티컬: 피부·두피, 반려동물 건강, 식물 관리, 인테리어 견적, 중고 시세 감정.
3. 해외 B2B 마이크로 SaaS의 한국판: 카카오 알림톡 결제실패 복구, 스마트스토어 리뷰 답변 자동화 등 "지루한" 영역.

---

## 트렌드 3. API 단가 붕괴 + Apple의 무료 온디바이스·PCC 추론

**근거**
- 프런티어급 LLM 토큰 가격은 2년 전의 약 1/5(70~85% 하락). [블로그] https://wavect.io/blog/llm-api-costs-2026-architecture-shift/ / 프런티어 토큰 가격 지수 18.7(2023.3 기준 대비 81.3% 하락, 2026-09-27). [블로그] https://benchlm.ai/llm-pricing-trends
- 저가 모델 예시: Gemini Flash급 입력 100만 토큰당 0.10달러 / 출력 0.40달러, DeepSeek V3.2 입력 0.27달러(캐시 0.07달러). [블로그] https://www.aimagicx.com/blog/llm-pricing-collapse-developer-guide-building-cheap-ai-2026 , https://deploybase.ai/articles/cost-per-token-over-time-how-llm-api-pricing-has-dropped
- **Apple WWDC 2026(6월 9일)**: Foundation Models 프레임워크를 오픈소스화하고, 온디바이스 모델에 이미지 입력(영수증·스크린샷·사물 인식)을 추가했다. 서드파티 모델(Claude, Gemini)도 같은 API로 묶었고, **App Store 신규 다운로드 200만 미만 개발자에게는 Private Cloud Compute의 Apple 서버 모델을 무료로 제공**한다. [블로그] https://dracode.dev/blog/2026-06-15-08-foundation-models-ios27-free-ai/ , https://dev.to/hariharanjagan/whats-new-in-apples-foundation-models-framework-at-wwdc-2026-5227 , https://rits.shanghai.nyu.edu/ai/apple-open-sources-its-foundation-models-framework-adds-claude-and-gemini/ (Apple 공식 원문은 2단계에서 확인 필요)

**왜 지금인가**
- 예산 100만원 이하인 1인 개발자에게 가장 큰 위험은 "사용자가 늘수록 API 비용이 늘어나는 것"이었다. iOS 27 + PCC 무료 정책으로, 소규모 개발자는 추론 비용 0원으로 AI 기능을 넣을 수 있게 됐다.
- 무료 사용자에게도 AI를 넉넉히 줄 수 있어 프리미엄(무료→유료) 구조가 경제적으로 성립한다.

**파생 기회**
1. iOS 전용 "추론비 0원" AI 앱: 온디바이스 이미지 이해로 영수증 가계부, 명함·서류 정리, 사진 칼로리 등.
2. 프라이버시·오프라인을 전면에 둔 AI 앱(일기, 상담형 저널, 건강 기록). "데이터가 폰 밖으로 나가지 않음"을 마케팅 포인트로.
3. 보유 앱 10개에 온디바이스 AI 기능을 일괄 탑재해 업데이트 → ASO 재노출 + 구독 전환율 개선.

---

## 트렌드 4. 실시간 음성 AI 단가 하락 → AI 전화응대/예약

**근거**
- OpenAI realtime 계열 가격 20% 인하, 2026-05-07 종량제 실시간 음성 모델 도입. 캐시 입력 100만 토큰당 0.40달러. gpt-realtime mini는 정가의 약 1/3. [블로그] https://www.elegantsoftwaresolutions.com/blog/ai-voice-agents-small-business-customer-service , https://www.layer3labs.io/guides/openai-realtime-api-pricing
- 해외 소상공인용 AI 리셉션 실비용: 분당 0.09~0.25달러, 월 500콜 미만 업장은 월 99~500달러. [블로그] https://autocalls.ai/article/ai-voice-agent-pricing
- 국내 경쟁 상황: KT AI 통화비서는 2만 개 이상 업소가 사용 중. [2차] https://www.newstheai.com/news/articleView.html?idxno=3986 / 정부의 전 국민 무료 "모두의 AI"가 카톡·전화로 예약·결제를 대행하며 10월부터 단계적으로 공개, 12월 출시 예정. 소상공인 예약·세무 처리와 개발자 수익 공유도 검토 중. [2차] 이데일리 — https://edaily.co.kr/News/Read?mediaCodeNo=257&newsId=03079926645576840 , 파이낸셜뉴스 — https://www.fnnews.com/news/202607161810292491 / 식당 AI 예약 전화 월 19,000원 서비스도 이미 등장. [블로그] https://claw-ops.com/blog/restaurant-ai-reservation

**왜 지금인가**
- 기술 원가로는 1인 사업이 가능해졌지만, 국내에서는 통신사(KT)와 정부("모두의 AI")가 범용 시장을 무료·저가로 장악하는 중이다. 범용 시장으로 정면 승부하기는 어렵다(**추정**).

**파생 기회**
1. 범용이 아닌 특정 업종 전용 음성 에이전트(예: 학원 상담·보강 예약, 펜션 예약·환불 규정 안내, 동물병원 접수). 업종별 FAQ·예약 시스템 연동이 차별점.
2. "모두의 AI" 에이전트 마켓플레이스에 들어가는 업종별 도구 공급자(정부 플랫폼을 유통 채널로 활용).
3. 통화 녹취를 요약해 CRM·카톡으로 후속 연락하는 B2B 유틸리티.

---

## 트렌드 5. 영상 생성 단가 하락 → AI UGC·숏폼 광고

**근거**
- 720p 영상 API 단가: Veo 3.1 Lite 초당 0.03달러, Kling 3.0 0.084~0.168달러, Sora 2 약 0.10달러. 월 100클립 기준 Kling 약 50달러. [블로그] https://devtk.ai/en/blog/ai-video-generation-pricing-2026/ , https://tokenmix.ai/blog/ai-video-generation-api
- 광고 영상 1편 제작비: 에이전시 100~500달러, UGC 크리에이터 평균 198달러(전년 대비 -44%), AI 도구 1~5달러. [블로그] https://sovran.ai/benchmarks/video-ad-production-cost
- AI UGC 광고 스타트업 Creatify 누적 1,900만 달러 투자 유치, Arcads 등 해외 다수. [블로그] https://startupintros.com/orgs/creatify-ai , https://www.arcads.ai/

**왜 지금인가**
- 영상 1편의 원가가 커피 한 잔 값 아래로 떨어졌다. 한국에는 스마트스토어·쿠팡 셀러가 매우 많지만, 이들이 한국어 숏폼 광고를 직접 만들 수 있는 도구는 해외 서비스 대비 현지화가 약하다(**추정**).

**파생 기회**
1. 스마트스토어 셀러용 "상품 URL → 한국어 숏폼 광고·상세페이지" 자동 생성 SaaS(크레딧 과금).
2. 로컬 매장용 릴스·쇼츠 자동 제작 구독(월 n편).
3. 보유 앱의 ASO·광고 소재 자동 생성에 먼저 써 보면서(도그푸딩) 상품화.

---

## 트렌드 6. 에이전트 유통 채널의 개방 — ChatGPT 앱/플러그인, 카카오 PlayMCP, "모두의 AI"

**근거**
- OpenAI Apps SDK(MCP 기반)로 만든 앱을 ChatGPT 디렉터리에 올릴 수 있다. 2026년 초 MCP Apps UI 표준을 적용했고, 2026-07-09 App directory가 Plugin directory로 바뀌었다. 승인된 앱은 Codex 플러그인으로도 배포된다. 수익화 도구와 Agentic Commerce Protocol(대화 안 결제)도 예고됐다. [1차] https://openai.com/index/developers-can-now-submit-apps-to-chatgpt/ / [블로그] https://www.poster.ly/guides/chatgpt-guide
- 카카오 PlayMCP: 국내 최초 MCP 오픈 플랫폼. 카카오 서비스 외에 외부 MCP 서버 약 200개가 등록돼 있고 누구나 등록할 수 있다. 오픈클로 연동 지원(2026-05). "MCP Player 10" 공모전은 10명에게 총 2,100만원 지원. [1차] https://www.kakaocorp.com/page/detail/11674?lang=ENG , https://www.kakaocorp.com/page/detail/12012?lang=ENG / 공모전 — https://www.wevity.com/index_university.php?c=find&s=_university&gub=1&cidx=21&gbn=viewok&gp=1&ix=103990
- 카카오톡 안 ChatGPT 챗봇(2026-06, 단체방에서 @ 멘션으로 호출). [2차] https://www.digitaltoday.co.kr/en/view/64293/kakao-launches-chatgpt-chatbot-feature-in-kakaotalk-for-in-chat-calling
- 정부 "모두의 AI"는 신뢰할 수 있는 AI 에이전트 유통 마켓플레이스와 생활 밀착형 에이전트·도구 개발을 지원할 계획이다. [2차] https://www.mt.co.kr/tech/2026/07/23/2026072215142737408

**왜 지금인가**
- 앱스토어 초창기처럼 새 유통 채널은 초기 진입자가 노출을 독점한다. PlayMCP의 외부 서버가 약 200개인 지금이 선점 구간이다.
- 1인 개발자에게 가장 비싼 것은 사용자 획득 비용인데, 이 채널들은 광고비 없이 노출될 수 있다.

**파생 기회**
1. 한국 데이터 MCP 앱: 정부지원사업·공고 검색, 부동산 실거래가, 법령·판례, 청약, 공공데이터 → ChatGPT·Claude·PlayMCP 동시 배포.
2. 보유 앱(예: 그로우온 목표 관리)의 MCP 버전 → "ChatGPT에서 내 목표 기록" 같은 새 유입 경로.
3. PlayMCP 공모전·모두의 AI 플래그십 프로젝트로 비희석 자금과 레퍼런스 확보.

---

## 트렌드 7. 네이버 AI 브리핑 확대 → GEO(생성형 검색 최적화) 수요

**근거**
- 네이버 AI 브리핑이 검색 결과 최상단에서 출처와 함께 요약을 제공하며 적용 범위가 확대되고 있다. Top10 밖 콘텐츠도 인용된다. [블로그] https://seonews.co.kr/naver-ai-briefing-geo-202605/ , https://seonews.co.kr/naver-search-report-june-2026/
- FAQ 스키마를 적용한 페이지가 AI 답변에 인용될 확률이 3.2배 높다는 주장. [블로그, 미검증] https://www.pageoneworks.com/article/naver-ai-briefing-optimization-guide-2026
- Sensor Tower 2026 보고서도 "AI가 쇼핑의 새 관문"이 되고 있다고 짚었다. [2차] https://www.theneuron.ai/explainer-articles/state-of-ai-2026-report-form-sensor-tower-ai-is-becoming-the-new-front-door-to-shopping/

**왜 지금인가**
- 소상공인과 중소 브랜드가 "AI 답변에 우리 가게가 나오는지"를 처음 걱정하기 시작한 단계다. 대행사는 생겨나고 있지만, 저가 셀프서비스 SaaS는 드물다(**추정**).

**파생 기회**
1. "우리 가게/브랜드가 네이버 AI 브리핑·ChatGPT·Perplexity에 언급되는가" 모니터링 + 개선 제안 SaaS(월 1~3만원대).
2. 플레이스·블로그 글을 GEO 구조(결론 먼저, FAQ)로 다시 쓰는 도구.
3. 앱 개발자용 "AI 검색 노출" ASO 확장 도구(자기 앱으로 도그푸딩 가능).

---

## 트렌드 8. AI 기본법 시행 — 표시·고지 의무와 계도기간

**근거**
- 「인공지능 발전과 신뢰 기반 조성 등에 관한 기본법」이 2026-01-22 시행됐다. 생성형·고영향 AI 제품·서비스 사업자는 이용자에게 AI 사용 사실을 미리 알리고, 결과물에 AI 생성 사실을 표시해야 한다(워터마크, 딥페이크 표시). [2차] 국민일보 — https://www.kmib.co.kr/article/view.asp?arcid=1768984300 , 헬로디디 — https://www.hellodd.com/news/articleView.html?idxno=110602
- 위반 시 시정명령과 최대 3,000만원 과태료. 1년 이상 계도기간을 두어 실제 부과는 빨라도 2027년 이후. AI를 단순히 도구로 쓰는 개인 이용자는 의무 대상이 아니다. [2차] 매일신문 2026-09-24 — https://www.imaeil.com/page/view/2026092412193369072 , [블로그] https://bh-law.kr/ko/news/column/ai-content-labeling-obligation-guide
- 정부는 통합안내지원센터를 운영하고 검·인증·영향평가 비용과 전문가 컨설팅을 지원한다. [2차] https://www.skax.co.kr/insight/trend/3666 , https://www.pwcconsulting.co.kr/ko/insights/ai-law.html
- 컨설팅 시장은 대형 펌(PwC, KPMG, SK AX)과 셀렉트스타 등이 세미나·컨설팅으로 선점 중이다. [2차] https://selectstar.ai/blog/notice/ai-basic-act-seminar-2026/ , https://kpmg.com/kr/ko/home/newsletter-channel/202505/team-story.html

**왜 지금인가**
- 대기업은 컨설팅을 사지만, 수천 개의 소규모 AI 앱·서비스 사업자(창업자 본인 포함)는 "무엇을 어디에 표시해야 하는지"를 싸고 빠르게 해결할 도구가 필요하다. 계도기간이 끝나는 2027년 초까지가 수요가 가장 큰 시기다(**추정**).
- 창업자는 이미 약관·개인정보 문서를 직접 작성해 온 경험이 있어 도메인 진입장벽이 낮다(이 저장소 이름도 growon-legal).

**파생 기회**
1. 소규모 AI 서비스용 "AI 기본법 셀프 체크 + 고지문·표시 문구 생성기"(웹 SaaS, 건당 또는 월 구독).
2. 앱·웹용 AI 생성물 표시/워터마크 SDK(iOS·Android·웹 컴포넌트, 메타데이터 삽입 포함).
3. 앱 개발자용 약관·개인정보처리방침·AI 고지 통합 생성기(앱스토어 심사 대응 포함).

---

## 트렌드 9. 정부 AI 지원사업 대규모 편성 — 수요기업·공급기업 양쪽 기회

**근거**
- 2026 AX 원스톱 바우처(과기정통부·NIPA): AI·클라우드·데이터를 통합 지원, 총 260억원, 과제당 약 13억원 내외·약 2년. 접수 2026-04-08~05-07, 추가 모집도 있었음. [1차] 기업마당 — https://www.bizinfo.go.kr/sii/siia/selectSIIA200Detail.do?pblancId=PBLN_000000000120085 , 과기정통부 추가모집 — https://www.msit.go.kr/bbs/view.do?sCode=user&nttSeqNo=3186756&bbsSeqNo=100
- 2026 데이터바우처 수요기업 모집. [1차] https://www.bizinfo.go.kr/sii/siia/selectSIIA200Detail.do?pblancId=PBLN_000000000119210
- 2026 혁신 소상공인 AI 활용지원(중기부): 신규 예산 143.6억원, AI 활용모델 구축 1,000개사, 사업화 680개사, 최대 4천만원. 접수 2026-06-12~07-03(마감). [1차] 중기부 통합공고 — https://mss.go.kr/site/smba/ex/bbs/View.do?cbIdx=86&bcIdx=1064370&parentSeq=1064370 / [블로그] https://www.omago.ai/ko/blog/korea-sme-ai-subsidies-2026
- 중기부 "AI로 매출 늘린 중소기업 우수사례 공모전"(2026-08-31). [2차] https://www.newspim.com/news/view/20260831001010
- 국가 AI 행동계획(인공지능 기본계획 2026~2028), 2026-02 국가인공지능전략위원회. [1차] https://smartcity.go.kr/wp-content/uploads/2026/03/%EC%95%88%EA%B1%B41%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD%EC%9D%B8%EA%B3%B5%EC%A7%80%EB%8A%A5%ED%96%89%EB%8F%99%EA%B3%84%ED%9A%8D%EC%9D%B8%EA%B3%B5%EC%A7%80%EB%8A%A5%EA%B8%B0%EB%B3%B8%EA%B3%84%ED%9A%8D20262028.pdf

**왜 지금인가**
- 2026년 사업 대부분은 접수가 끝났다. 2027년 공고는 통상 1~2분기에 나오므로(**추정**, 예년 패턴), 지금부터 준비하면 공급기업 등록이나 수요기업 매칭 서비스를 공고 시점에 맞춰 출시할 수 있다.
- 소상공인 1,000곳 이상이 "AI를 도입하라는 돈"을 받았거나 받으려 한다. 즉 저가 AI 도구를 살 이유와 예산이 생겼다.

**파생 기회**
1. 정부 AI 지원사업 매칭 + 사업계획서 초안 작성 AI(소상공인·초기 창업자 대상). 기존 공고 검색 서비스와의 차별점 검증 필요.
2. 바우처·지원사업 공급기업으로 등록할 수 있는 저가 AI 패키지(예: 업종별 챗봇 + 콘텐츠 자동화).
3. 창업자 본인의 비희석 자금 확보: 예비·초기창업패키지, PlayMCP 공모전, 모두의 AI 플래그십 프로젝트.

---

## 트렌드 10. (참고) 국내 AI 투자 쏠림

**근거**
- 2026년 상반기 국내 스타트업 투자 7조 8,005억원으로 2025년 연간 총액(6조 9,358억원)을 넘어섰다. AI·로보틱스 2조 6,850억원(+485.2% YoY), 시드 투자액의 91.5%가 AI·로보틱스. 100억원 이상 딜이 전체 금액의 93%. [2차] 플래텀 — https://platum.kr/archives/290277 , 와우테일 2026-06-24 — https://wowtale.net/2026/06/24/260584/ , 더브이씨 — https://thevc.kr/discussions/korea_startup_funding_2026_q1

**시사점**
- 자본은 딥테크와 대형 딜로 몰린다. 1인 저예산 창업자는 VC 경쟁보다 "매출 먼저 + 정부 비희석 자금" 경로가 현실적이다(**추정**).
- 반대로 VC 투자를 받은 국내 AI 앱 스타트업이 늘어나므로, B2C 범용 AI 앱(예: AI 비서, AI 캐릭터 채팅)은 피하는 편이 낫다.

---

## 주의해야 할 역풍 (리스크 메모)
- **플랫폼 흡수 위험**: ChatGPT·Claude·Gemini·네이버 Agent N·카카오가 범용 기능(요약, 번역, 예약 대행)을 기본 탑재한다. "모델 회사가 다음 업데이트로 넣을 기능"은 피해야 한다.
- **정부 무료 서비스와의 충돌**: "모두의 AI"(12월 출시 예정)가 대국민 예약·민원·생활 업무를 무료로 처리하면, 범용 B2C 에이전트는 어려워진다.
- **AI 앱 리텐션**: 12개월 리텐션 21%. 데이터 축적형·업무 필수형이 아니면 LTV가 낮다.
- **한국 고유 규제**: 의료·법률 조언, 개인정보(민감정보), 녹취 고지 등은 버티컬마다 별도로 검토해야 한다.

---

## 주목할 기회 Top 5

1. **AI 기본법 셀프 컴플라이언스 툴킷** — 소규모 AI 앱·서비스 사업자용 고지문·생성물 표시 생성기 + 표시 SDK. 계도기간 종료(2027 초) 전이 적기이고, 창업자의 약관 작성 경험과 맞물린다.
2. **"추론비 0원" 한국형 사진 AI 앱(Cal AI 타임머신)** — Apple PCC 무료 정책과 온디바이스 이미지 이해로 한식 칼로리 등 사진 → 기록 → 리포트 구독 앱을 만든다. 보유 앱 10개와 출시 파이프라인을 그대로 활용할 수 있다.
3. **한국 데이터 MCP 앱으로 에이전트 채널 선점** — 정부지원사업·부동산·법령 등 한국 데이터를 ChatGPT 플러그인과 카카오 PlayMCP(외부 서버 약 200개)에 동시 배포한다. 광고비 없이 노출되고 공모전 자금도 노릴 수 있다.
4. **소상공인 GEO(네이버 AI 브리핑) 모니터링·최적화 SaaS** — "AI 답변에 우리 가게가 나오나?"를 진단하고 콘텐츠를 다시 써 준다. 저가 셀프서비스 시장은 아직 비어 있다(추정).
5. **스마트스토어 셀러용 한국어 AI 숏폼 광고 생성기** — 영상 API 초당 0.03달러로 원가가 붕괴했다. 상품 URL을 넣으면 숏폼·상세페이지가 나오는 크레딧 과금형 서비스. (차순위: 특정 업종 전용 AI 전화응대, 정부지원사업 매칭·계획서 AI)

> 다음 단계 제안: Top 5 각각에 대해 (a) 국내 경쟁 서비스 실사, (b) 타깃 고객 10명 인터뷰 또는 커뮤니티 수요 확인, (c) 2주 MVP 범위 정의.
