# Codex Rises, Claude Meters Programmatic Usage

**원문 URL**: https://www.latent.space/p/ainews-codex-rises-claude-meters
**번역일**: 2026-05-14 06:18
**발행일**: 2026-05-14

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Codex의 부상, Claude 프로그래매틱 사용량에 미터링 적용

### 조용한 하루, 주요 코딩 에이전트들의 장기적인 추세에 대해 보고합니다
ShareIt GPT 5.5 출시 이후 지난 3주간은 두 도시 이야기였습니다. 금융 업계에서는 Anthropic의 성장과 10월 IPO 가능성을 앞둔 CFO에 매료된 반면, AI 엔지니어들 사이에서는 Codex 지지 정서가 눈에 띄게 증가했습니다. 이는 GPT 5.5가 (일부 시나리오에서는 Mythos급으로) 정말 좋은 모델이라는 점, Codex for Everything Else의 출시, 그리고 오늘 사설의 계기가 된 세 번째 요인인 더 관대한 제한이 복합적으로 작용한 결과일 것입니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/1f3bb92f-f1bd-4329-9b9c-64c681eeec378_1290x874.png)
Claude의 가격 정책 변경에 대한 메시지는 전반적으로 잘 전달되었지만, 대체 하네스 사용자들은 듣고 싶지 않은 내용이었습니다. 이제 모든 Claude 구독은 Claude 구독 요금제 금액과 동일한 월별 API 토큰 크레딧을 받습니다. 즉, 200달러를 지불하면 Claude.ai 및 Claude Code와 같은 Anthropic 소유 하네스에서 Claude를 사용하는 데 자체 제한이 있는 Claude 구독("인터랙티브 사용량")과 claude-p, OpenClaw 등을 포함한 다른 모든 곳에서 Claude를 사용하는 데 사용할 수 있는 200달러 상당의 API 크레딧("프로그래매틱 사용량")을 모두 얻게 됩니다.
만약 처음부터 이런 식으로 작동했다면, 매우 좋은 거래로 여겨졌을 것입니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/148215c3-6a2e-4a77-b243-630d5c9c7247_1228x1640.png)
그러나 역사적인 보조금/가격 이점(API 가격에서 70-90% 할인으로 추정) 때문에 사람들은 이를 일종의 "러그 풀"로 보고 있습니다. 하지만 OpenClaw, OpenCode에 대한 선택적 타겟팅과 덜 인기 있는 하네스의 불확실한 상태에 비해 공식 정책이 마련된 것은 좋은 일입니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/041d6b0a-7e96-82ad-750ed4e73f25_1208x1394.png)
이러한 헤드라인이 OpenAI가 기업 전환 프로모션을 시작한 날과 겹친 것은 놀라운 우연의 일치입니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/8449d76b-2f12-4dde-a825-744697b02502_1192x1116.png)
결국, 어느 쪽이든 과도하게 해석하는 것은 경계해야 합니다. 두 연구소 모두 매우 잘하고 있으며, 이는 수십 년 된 산업을 뒤흔들면서 코딩의 미래를 발명하고 최적의 가격을 찾아가는 사람들의 정상적인 가격 변동입니다. Anthropic은 처음에는 더 관대했지만, 이제 Claude Code가 에이전트 하네스로서 지속 가능한 브랜드와 영향력을 갖게 되면서 Anthropic은 자체 도구에 가장 유리한 가격을 책정하고 다른 모든 것에 미터링을 적용하고 있습니다. 반면 도전자로서의 Codex는 모든 것에 더 관대하게 접근하고 있습니다.
아마도 하드웨어가 운명일 수도 있고, 아니면 이것이 "맨데이트 이퀴녹스"라는 6개월 교대 주기의 일부일 수도 있습니다.

![X avatar for @irl_danB](https://pbs.substack.com/profile_images/1998260537583357952/yiIzRggQ.png)
> 2026년 5월 12일~5월 13일 AI 뉴스입니다. 12개의 서브레딧, 544개의 트위터를 확인했으며 더 이상 디스코드는 확인하지 않았습니다. AINews 웹사이트에서 지난 호를 모두 검색할 수 있습니다. 참고로 AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
에이전트 인프라, 하네스 및 개발자 플랫폼
- Cline, LangChain, Notion, Cursor는 모두 에이전트 플랫폼 영역으로 더 깊이 진출했습니다. Cline은 재구축된 Cline SDK와 TUI, 에이전트 팀, 예약된 작업, 커넥터를 갖춘 CLI를 오픈소스화하여 자체 하네스를 맞춤형 코딩 에이전트를 위한 재사용 가능한 기반으로 포지셔닝했습니다. LangChain은 Interrupt에서 LangSmith Engine, SmithDB, Sandboxes, Managed Deep Agents, LLM Gateway, Context Hub, Deep Agents 0.6 등 에이전트 라이프사이클 인프라를 대량으로 출시했습니다. 기술적으로 가장 주목할 만한 부분은 중첩되고 장기 실행되는 대규모 페이로드를 가진 트레이스를 위한 목적에 맞게 구축된 관측 가능성 데이터베이스인 SmithDB입니다. 이는 주요 워크로드에서 12~15배 더 빠른 접근을 제공한다고 보고되었습니다. 팀은 Apache DataFusion과 Vortex를 기반으로 구축되었다고 말합니다. 이와 동시에 Notion의 External Agents API는 Claude, Codex, Cursor, Decagon, Warp, Devin과 같은 서드파티 에이전트가 또 다른 사일로가 아닌 공유 가능하고 검토 가능한 컨텍스트 레이어로서 Notion 내에서 직접 작동할 수 있도록 합니다. Cursor는 클론된 레포, 의존성, 버전 기록, 롤백, 범위가 지정된 이그레스, 격리된 시크릿을 포함한 완전히 구성된 개발 환경으로 클라우드 에이전트를 확장했습니다.
- 에이전트 UX는 채팅보다는 장기 실행 상태, 스트리밍 및 오케스트레이션에 점점 더 중점을 둡니다. 여러 출시가 동일한 설계 방향으로 수렴했습니다. Duet Agent는 몇 주 또는 몇 달 동안 지속되는 작업을 위한 상태 머신 하네스를 제안하며, 압축을 부모/하위 에이전트 조정 및 메모리로 대체합니다. LangChain의 오픈소스 업데이트는 스트리밍 타입 프로젝션, 체크포인트 저장, 코드 인터프리터, 하네스 프로필 및 모델별 튜닝을 추가했으며, 이 모든 것은 일반 토큰보다 더 풍부한 에이전트 이벤트 스트림을 목표로 합니다. Tabracadabra는 자동 완성에서 모든 텍스트 상자의 컨텍스트 인식 어시스턴트로 전환했으며, VS Code는 에이전트 창과 더 나은 다중 프로젝트 작업 검토 기능을 도입했습니다. 이러한 릴리스 전반의 아키텍처적 메시지는 프로덕션 에이전트가 상태 비저장 프롬프트/응답 루프보다는 내구성 있는 실행, 검사 가능한 중간 상태 및 도구 네이티브 UI 표면을 점점 더 필요로 한다는 것입니다.
모델 학습, 아키텍처 및 데이터 효율성
- 사전 학습 효율성과 아키텍처 실험은 가장 강력한 연구 흐름이었습니다. Nous Research의 Token Superposition Training은 사전 학습의 초기 단계를 수정하여 모델이 표준 다음 토큰 예측으로 돌아가기 전에 연속적인 토큰 묶음을 읽고 예측하도록 합니다. 그들은 동일한 FLOPs에서 인퍼런스 시 아키텍처 변경 없이 2~3배의 실제 시간 속도 향상을 보고했으며, 2억 7천만 개에서 30억 개 밀집 모델과 100억 개-A1B MoE 모델에서 검증되었습니다. Jonas Geiping 외 연구진은 현재 메시지 기반/채팅 학습이 에이전트를 단일 스트림으로 과도하게 제한한다고 주장하며, 더 낮은 레이턴시, 더 깔끔한 관심사 분리, 더 명확한 병렬 추론/도구 사용을 주장하는 멀티스트림 LLM 논문을 발표했습니다. 논문과 코드는 여기에 링크되어 있습니다. δ-mem은 고정된 풀 어텐션 백본에 연결된 외부 온라인 연관 메모리를 제안했으며, 8x8 상태가 평균 점수를 1.10배 향상시키고 비-δ-mem 기준선을 1.15배 능가하며, 메모리 집약적 벤치마크에서 더 큰 이득을 보인다고 보고되었습니다.
- 후처리/압축 및 데이터 큐레이션 또한 주목할 만한 결과를 낳았습니다. NVIDIA의 Star Elastic은 한 번의 후처리 실행으로 추론 모델 크기 제품군을 도출할 수 있으며, 제품군을 사전 학습하는 것보다 360배 낮은 비용으로 SOTA 압축보다 7배 우수하다고 주장합니다. Siddharth Joshi와 Pratyush Maini가 강조한 Datology의 VLM 작업은 데이터 큐레이션만으로도 주요 멀티모달 이득을 얻을 수 있다고 주장합니다. 2B 모델에서 20개 공개 VLM 벤치마크 전반에 걸쳐 +11.7점을 달성하여 InternVL3.5-2B를 약 10점 차이로 능가했으며, 학습 컴퓨팅은 약 17배 적게 사용했습니다. 또한 Qwen3-VL-4B보다 3.3배 낮은 응답 FLOPs로 프론티어 모델에 가까운 4B 성능을 달성했습니다. 오픈 데이터 측면에서 Percy Liang은 다음 Marin 실행에 이미 18조 토큰이 포함되어 있으며, 더 많은 사전 학습, 중간 학습 및 SFT 데이터를 계속 찾고 있다고 말했으며, 동반 토큰 뷰어가 여기에 공유되었습니다.
- 오픈 평가 및 데이터셋 작업은 모델 구축과 함께 성숙하고 있습니다. Kevin Li의 SWE-ZERO-12M-trajectories는 가장 큰 오픈 에이전틱 트레이스 데이터셋으로 포지셔닝되었습니다. 1120억 토큰, 1200만 트레이스, 12만 2천 개의 PR, 3천 개의 레포, 16개 언어를 포함합니다. Victor Mustar는 llama-eval을 더 비교 가능한 llama.cpp 커뮤니티 평가를 향한 한 단계로 지적했습니다. 한편, Steve Rabinovich와 Sayash Kapoor는 더 강력한 에이전트가 숨겨진 벤치마크 버그와 보상 해킹 경로를 드러내기 때문에 신뢰할 수 있는 에이전트 평가는 결과만 보는 지표가 아닌 로그 분석을 필요로 한다고 주장했습니다.
기업 AI 가격 책정, 플랫폼 경쟁 및 유통
- Anthropic 대 OpenAI 경쟁은 기업 유통 및 개발자 록인(lock-in)을 중심으로 심화되었습니다. Andrew Curran이 인용한 Ramp 데이터는 4월에 Anthropic이 기업의 34.4%, OpenAI가 32.3%를 차지하여 기업 채택에서 처음으로 명백한 선두 변화를 보여주었습니다. The Rundown도 동일한 수치를 확대했습니다. 동시에 Anthropic은 요금제 경제성을 변경했습니다. ClaudeDevs는 유료 Claude 요금제가 Agent SDK, claude -p, GitHub Actions 및 서드파티 SDK 앱 전반에 걸쳐 프로그래매틱 사용량을 위한 전용 월별 크레딧을 받게 될 것이라고 발표했습니다. 이는 파워 유저들에게 구독 보조 하네스에 대한 주요 제한으로 즉시 해석되었으며, Theo, Jeremy Howard, Matt Pocock, Omar Sanseviero로부터 비판을 받았습니다. Anthropic은 이전에 발표된 2배 5시간 제한 증가에 추가하여 7월 13일까지 Claude Code 주간 제한을 별도로 50% 증가시켜 이러한 반발을 부분적으로 상쇄했습니다.
- OpenAI는 Codex 기업 인센티브로 공격적으로 대응했습니다. OpenAI Devs와 Sam Altman은 향후 30일 이내에 전환하는 기업 고객에게 두 달간의 무료 Codex 사용을 제공했습니다. OpenAI는 또한 로컬 파일 시스템/도구 접근 권한으로 코딩 에이전트를 안전하게 실행하는 데 필요한 로컬 사용자, 방화벽 규칙, ACL, 쓰기 제한 토큰, DPAPI 및 헬퍼 실행 파일의 조합을 설명하는 Windows 샌드박스 설계 보고서를 포함하여 더 많은 기술 플랫폼 세부 정보를 발표했습니다. 이제 경쟁 역학은 "최고의 모델이 승리"하는 것보다는 보조금 + 워크플로우 제어 + 하네스 호환성에 더 가깝습니다.
- 기업 채택은 런타임/보안 보장과 점점 더 밀접하게 연결되고 있습니다. Perplexity는 VPC 수준 분리, 단기 프록시 토큰, 에이전트 작업 전 외부 콘텐츠 스캔을 포함하는 하드웨어 격리 샌드박스 아키텍처를 설명했으며, 암호화 및 자동 삭제에 대한 추가 세부 정보도 제공했습니다. Aravind Srinivas는 이를 Perplexity가 기업 지식/연구 플랫폼이 되는 데 필수적인 기반으로 보았습니다. 더 넓은 패턴은 다음과 같습니다. 에이전트 공급업체는 더 이상 지능만을 판매하는 것이 아닙니다. 그들은 경계가 있는 실행 환경을 판매하고 있습니다.
자율 과학, 사이버 역량 및 로봇 공학
- 재귀적 자기 개선은 아이디어에서 스타트업 클러스터로 이동했습니다. 가장 큰 단일 메타 테마는 과학을 자동화하고 안전하게 스스로 개선하는 AI를 구축하기 위해 설립된 Recursive의 출시였습니다. Richard Socher, Josh Tobin, Dominik Schmidt, Jenny Zhang, Shengran Hu의 출시 게시물은 개방성, AI 과학자 및 연구 자동화 작업에서 영감을 받은 팀을 시사합니다. 인접한 작업으로, Adaption의 AutoScientist는 프론티어 연구소 외부에서 전체 학습-연구 루프를 자동화하는 것을 목표로 하며, Sarah Hooker는 대부분의 모델 학습 실패가 단순한 컴퓨팅 부족보다는 연구 루프의 취약성 때문이라고 주장합니다.
- 사이버 역량 평가는 계속해서 심화되고 있습니다. 영국 AI 보안 연구소는 프론티어 모델이 완료할 수 있는 사이버 작업의 길이가 몇 달마다 두 배로 증가하고 있으며, 최신 모델이 이전 추세를 능가하고 있다고 말했습니다. Anthropic/Glasswing의 Logan Graham은 Claude Mythos Preview가 Cooling Tower를 포함한 AISI 엔드투엔드 사이버 레인지를 모두 해결한 최초의 모델이며, 연구소의 250만 토큰 제한 내에서 모든 작업을 완료한 유일한 모델이라고 말했습니다. XBOW는 "토큰 단위로 전례 없는 정밀도"를 발견했다고 보고되었으며, 파트너 사용으로 몇 주 만에 수천 개의 높음/치명적 취약점이 드러났다고 합니다. scaling01의 독립적인 논평은 새로운 Mythos 버전이 사이버 레인지를 10번 중 6번 완료한 반면, 프리뷰 기준선은 10번 중 3번 완료했다고 주장했습니다.
- 로봇 공학은 구체적인 장기적 배포 데모를 선보였습니다. Figure의 Brett Adcock은 Helix-02를 사용하여 소포 분류에서 8시간 완전 자율 교대 근무를 수행하는 휴머노이드 로봇을 라이브스트림으로 공개했습니다. 후속 세부 정보에 따르면 로봇은 카메라 픽셀에서 추론하고, 인간과 비슷한 수준으로 작동(~패키지당 3초)하며, 온디바이스 인퍼런스를 수행하고, 네트워크화된 플릿으로 조정하며, 배터리 부족 시 자율적으로 교체하고, 필요할 때 자가 진단/유지 보수로 페일오버합니다. 이는 짧은 벤치마크 클립이 아닌 다중 로봇, 장시간, 인간 개입 없는 오케스트레이션의 더 명확한 공개 시연 중 하나입니다.
최고 인기 트윗 (참여도 기준)
- Claude Code 가격 및 제한: @ClaudeDevs의 50% 더 높은 주간 제한 발표, @ClaudeDevs의 프로그래매틱 크레딧 발표, 그리고 @theo로부터 이어진 개발자 반발은 당일 가장 중요한 개발자 이야기로 가격 정책을 만들었습니다.
- Codex 기업 공략: @sama가 전환 고객을 위한 두 달 무료 Codex 사용을 제안하고 @OpenAIDevs의 기업 대상 행동 촉구는 이례적으로 직접적인 시장 진출 반격 신호였습니다.
- Figure의 8시간 휴머노이드 교대 근무: @adcock_brett의 라이브스트림 게시물은 엄청난 관심을 끌었으며, 명확한 기술적 내용이 있는 몇 안 되는 바이럴 게시물 중 하나입니다.
- Cline SDK 출시: @cline의 SDK 출시는 오픈 코딩 에이전트 하네스에 대한 수요를 반영하며 가장 높은 참여도를 보인 진정한 기술 출시 중 하나였습니다.
- Token Superposition Training: @NousResearch의 TST 게시물은 널리 퍼진 희귀한 사전 학습 방법 트윗으로 두드러졌습니다. 이는 추론 시 아키텍처 변경 없이 2~3배의 학습 속도 향상이라는 주장이 구체적이고 경제적으로 중요하기 때문일 것입니다.

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. 효율적인 온디바이스 LLM 인퍼런스

## 7일 무료 체험으로 계속 읽으세요
이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하려면 Latent.Space를 구독하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-codex-rises-claude-meters&utm_source=paywall-free-trial&utm_medium=web&utm_content=197626124&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-codex-rises-claude-meters&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
