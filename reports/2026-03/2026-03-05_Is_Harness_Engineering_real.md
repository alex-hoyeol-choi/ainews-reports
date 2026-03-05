# Is Harness Engineering real?

**원문 URL**: https://www.latent.space/p/ainews-is-harness-engineering-real
**번역일**: 2026-03-05 07:28
**발행일**: 2026-03-05

---

[https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] 하네스 엔지니어링은 실재하는가?

### 조용한 날은 AI 엔지니어링의 핵심적인 논쟁에 대해 숙고하게 합니다.
제가 금융업에 종사하던 시절 흔했던 논쟁은 사람의 가치와 자리(seat)의 가치에 관한 것이었습니다. 한 트레이더가 3백만 달러의 수익을 냈다면, 그중 얼마가 그녀의 기술 때문이었고, 얼마가 그녀가 속한 직위/기관/브랜드 때문이었으며, 일반적으로 유능한 사람이라면 누구든 같은 결과를 낼 수 있었을까요?

같은 논쟁이 현재 에이전트 엔지니어링의 시스템 하위 집합이자 Agent Labs의 주요 업무인 "하네스 엔지니어링" 분야에서 격렬하게 벌어지고 있습니다. 핵심적인 대립은 Big Model과 Big Harness 사이에 있습니다. [여러분 모두가 아는 한 AI 프레임워크 창립자]가 언젠가 OpenAI 행사에서 제게 털어놓았습니다: “이 사람들이 제가 존재하기를 원하는지조차 모르겠습니다.”

> 여담: 하네스를 정의해봅시다 — “모든 엔지니어링 분야에서 하네스는 동일한 개념입니다: 구성 요소를 연결하고, 보호하며, 오케스트레이션하는 계층 — 그 자체로 작업을 수행하지는 않습니다.”

그리고 Big Model 진영 사람들과 이야기해보면, 정말로 그들의 입장을 알 수 있습니다:
- Boris Cherny와 Cat Wu가 출연한 모든 팟캐스트는 Claude Code의 하네스가 얼마나 최소한인지를 강조합니다. 이는 그들의 역할이 주로 모델 제작자만이 가장 잘 아는 방식으로 모델이 온전한 능력을 발휘하도록 하는 것임을 의미합니다:
Boris: “소스 코드에 딱히 비밀스러운 건 없다고 말하고 싶어요. 그리고 분명히 전부 JavaScript라서 그냥 디컴파일할 수 있습니다. 컴파일은 이미 공개되어 있죠. 아주 흥미롭습니다. 네. 그리고 일반적으로 저희 접근 방식은, 아시다시피, 모든 비법은 모델에 있습니다. 이것은 모델 위에 가능한 가장 얇은 래퍼(wrapper)입니다. 말 그대로 이보다 더 최소한으로 만들 수는 없었어요. 이게 가장 최소한의 것입니다.Cat [01:09:21]: 제 생각에는 의도적으로 가장 단순하게 만든 것입니다.Boris [01:09:25]: 그래서 더 단순해졌어요. 계속 단순해졌죠. 더 복잡해지지 않습니다. 저희는 아마 3주, 4주마다 처음부터 다시 작성했을 겁니다. 그리고 모든 것이, 테세우스의 배와 같아요, 그렇죠? 모든 부품이 계속 교체되고, Claude가 자체 코드를 너무 잘 작성하기 때문입니다.”
- OpenAI의 하네스 엔지니어링에 대한 자체 글은 (Codex 팀의 곧 출연할 게스트 Ryan Lopopolo와 함께) 시작하기가 얼마나 간단한지를 강조합니다. 물론, OpenClaw의 "임원 영입(execuhire)"으로 OpenAI는 이제 세계에서 가장 성공적인 오픈소스 하네스의 주요 투자자가 되었습니다.
- Noam Brown: “추론 모델이 등장하기 전에는 GPT-4o나 비추론 모델에 많은 호출을 하여 추론 동작을 얻으려는 에이전틱 시스템을 엔지니어링하는 데 많은 노력이 들어갔습니다. 그런데 알고 보니 우리는 그냥 추론 모델을 만들었고, 이 복잡한 동작은 필요하지 않습니다. 사실, 여러 면에서 더 나빠지기도 합니다. 마치 스캐폴딩 없이 추론 모델에 같은 질문을 주면 그냥 해내는 것과 같습니다. 그래서 사람들은 지금 추론 모델 위에 스캐폴딩을 구축하고 있습니다. 하지만 제 생각에는 여러 면에서 그러한 스캐폴드 또한 추론 모델과 전반적으로 더 유능해지는 모델에 의해 대체될 것입니다. 마찬가지로, 모델 라우터와 같은 것들도, 우리는 단일 통합 모델이 존재하는 세상으로 나아가고 싶다고 꽤 공개적으로 말해왔습니다. 그리고 그런 세상에서는 모델 위에 라우터가 필요하지 않을 것입니다.”
- METR은 Claude Code와 Codex가 기본적인 스캐폴딩을 능가하지 못한다고 말합니다:
- Scale AI의 SWE-Atlas는 Opus 4.6이 일반적인 SWE-Agent보다 Claude Code에서 2.5점 더 나은 성능을 보이지만, GPT 5.2의 경우 그 반대이며, 선택하는 하네스가 본질적으로 오차 범위 내의 노이즈임을 밝혀냈습니다:

하지만. Big Harness 진영 사람들은 동의하지 않습니다:
- 하네스가 곧 제품입니다: 모든 프로덕션 에이전트는 이 핵심 루프로 수렴합니다:
```
while (model returns tool calls): execute tool → capture result → append to context → call model again
```
이것이 전부입니다. Claude Code, Cursor의 에이전트, 그리고 Manus의 전체 아키텍처가 이 루프 안에 들어맞습니다.
- Jerry Liu: “모델 하네스가 전부입니다 — AI에서 가치를 얻는 가장 큰 장벽은 모델을 컨텍스트 및 워크플로우 엔지니어링하는 자신의 능력입니다. 이는 사용하는 도구가 수평적일수록 *특히* 더 그렇습니다.”
- "Improving 15 LLMs at Coding in One Afternoon. Only the Harness Changed"는 하네스(Pi)를 최적화할 때 모든 모델에서 극적인 개선을 보여줍니다.

분명히 Big Harness 진영 사람들은 자신들의 하네스를 팔려고 하고, Big Model 진영 사람들은 자신들의 모델을 팔려고 합니다. ML/AI 산업은 항상 양쪽 모두 가치 있다고 말하는 다소 온건한 "복합 AI" 논쟁을 벌여왔습니다. 하지만 시대가 변하고 있을지도 모릅니다.

Latent Space에서는 우리는 Bitter Lesson을 매우, 매우 존중해왔습니다. 하지만 Agent Labs의 주장이 점차 현실화되면서 (현재 Cursor의 가치는 500억 달러에 달합니다) 우리는 "하네스 엔지니어링"이 진정한 가치를 가지고 있음을 인정하고 있습니다. AIE Europe은 이제 세계 최초의 하네스 엔지니어링 트랙을 운영하고 있으며, 이 논쟁에 관심이 있다면 참여해야 합니다.

---
> 2026년 3월 3일~3월 4일 AI 뉴스. 저희는 12개의 서브레딧, 544개의 트위터, 24개의 디스코드(264개 채널, 14242개 메시지)를 확인했습니다. 예상 절약 독서 시간 (분당 200단어 기준): 1397분. AINews 웹사이트에서 지난 모든 호를 검색할 수 있습니다. 참고로, AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
프론티어 모델 출시: Gemini 3.1 Flash-Lite, GPT-5.4 루머, 그리고 "에이전트 우선" 제품 포지셔닝
- Gemini 3.1 Flash-Lite 포지셔닝 (속도/비용): Demis Hassabis는 Gemini 3.1 Flash-Lite를 성능 면에서 "놀랍도록 빠르고 비용 효율적"이라고 언급하며 —모델 라인업을 순수한 프론티어 점수보다는 레이턴시와 기능당 비용에 맞춰 명확히 설정했습니다 ([tweet](https://twitter.com/demishassabis/status/1764601119794026852)). 관련 제품 소식으로는 NotebookLM이 "가장 좋아하는 AI 도구"로 부각되었고 ([tweet](https://twitter.com/jackk/status/1764585789643440539)) NotebookLM Studio의 주요 신기능인 Cinematic Video Overviews는 Ultra 사용자들을 위해 사용자 소스에서 맞춤형 몰입형 비디오를 생성합니다 ([tweet](https://twitter.com/jackk/status/1764604925761358040)).
- GPT-5.4 유출 소식 (The Information): 여러 트윗에서 GPT-5.4가 약 1M 토큰 컨텍스트 윈도우와 "몇 시간 동안 생각할 수 있는" 새로운 "극단적 추론 모드"를 탑재하여 출시될 것이라는 보고서가 확산되고 있습니다. 이는 장기 에이전틱 워크플로우와 복잡한 작업의 오류율 감소를 목표로 합니다 ([tweet](https://twitter.com/TheInformation/status/1764593414909876356), [tweet](https://twitter.com/rowancheung/status/1764595603833202970), [tweet](https://twitter.com/alexalbert_/status/1764600216506306893)). 또한 OpenAI가 더 빈번한 (월별) 모델 업데이트로 전환하고 있다는 추측도 있습니다 ([tweet](https://twitter.com/gregisenberg/status/1764600122949703908)). 별도로, 한 아레나 관찰자는 “GPT-5.4가 아레나에 도착했다”고 주장하며, 이는 임박한 출시 시기를 암시합니다 ([tweet](https://twitter.com/lmsysorg/status/1764609249764567207)). 이 모든 정보는 OpenAI의 확인이 있기 전까지는 미확인으로 간주해야 합니다.
- Claude는 코딩뿐만 아니라 "에이전트 동작" 리더: Nat Lambert는 논의가 Anthropic이 "코드에 올인하는 것"에서 일반적인 에이전트 동작에서의 선두 위치로 전환되어야 한다고 주장합니다. 이는 코딩 능력은 상품화되겠지만 에이전트의 견고성은 그렇지 않을 것임을 암시합니다 ([tweet](https://twitter.com/natolambert/status/1764585694770653245)). MathArena 평가는 한 가지 데이터 포인트를 추가합니다: Claude Opus 4.6은 전반적으로 강력하지만 시각적 수학에는 약하며, 평가 비용이 많이 듭니다 (약 8천 달러로 주장됨) ([tweet](https://twitter.com/MathArena_AI/status/1764585694770653245)).

---

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-is-harness-engineering-real&utm_source=paywall-free-trial&utm_medium=web&utm_content=189942098&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-is-harness-engineering-real&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
