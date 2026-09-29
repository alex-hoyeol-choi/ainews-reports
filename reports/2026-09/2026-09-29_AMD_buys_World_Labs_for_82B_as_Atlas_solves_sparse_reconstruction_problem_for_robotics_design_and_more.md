# AMD buys World Labs for $8.2B, as Atlas solves sparse reconstruction problem for robotics, design and more

**원문 URL**: https://www.latent.space/p/ainews-amd-buys-world-labs-for-82b
**번역일**: 2026-09-29 06:19
**발행일**: 2026-09-29

---

[AINews] AMD가 World Labs를 82억 달러에 인수, Atlas는 로봇 공학, 디자인 등을 위한 희소 재구성 문제를 해결합니다

### 팀에 축하드립니다!
2026년 9월 29일 공유 공식 발표는 조심스럽지만, AMD는 상장 기업이므로 인수 가격을 알 수 있습니다. 저희는 1년도 채 되지 않아 이들을 다룬 적이 있습니다:
Fei Fei는 주요 이유를 암시하는 멋진 회고 블로그 게시물을 올렸습니다:
> 2024년 설립 이래, World Labs는 창작 작업부터 디자인에 이르기까지 모든 분야에서 선도적인 AI 공간 지능 역량을 구축해 왔습니다. 저희는 이미지, 비디오 및 공간 재구성을 위한 세계 최고 수준의 모델 학습 팀을 만들었습니다. 그리고 SceniX 인수를 통해 로봇 공학 시뮬레이션을 위한 업계 선도적인 역량을 구축하고 있습니다. 최근 저희는 공간 지능의 핵심적인 미해결 문제인 새로운 카메라 뷰 예측을 해결하는 최초의 옴니 모델 아키텍처인 Atlas를 출시했습니다. LLM이 한 줄의 텍스트에서 다음 토큰을 예측할 수 있듯이, Atlas는 2D 이미지 입력에서 다음 뷰를 예측할 수 있도록 처음부터 학습되었으며, 특수 모델보다도 SOTA 결과를 능가합니다. 이는 생성 모델과 다중 시점 기하학을 결합하여 컴퓨터 비전 분야의 오랜 문제인 희소 재구성을 본질적으로 해결했습니다. 이는 디자인 및 엔지니어링부터 과학 및 로봇 공학에 이르기까지 직접적이고 광범위한 영향을 미칩니다. 저희는 로봇 공학을 위한 RL 환경, 치료 및 엔터테인먼트를 위한 장면 생성, 부동산, 디자인 및 건설을 위한 실제 세계 재구성 등 수많은 분야에서 Atlas에 대한 엄청난 관심을 확인했습니다.
오늘 공개된 저희 Claude Code 팟캐스트도 확인해 보세요:
[Claude Code의 다음 시대 — Thariq Shihipar, Anthropic](https://www.latent.space/p/thariq)
![Claude Code’s Next Era — Thariq Shihipar, Anthropic](https://substack-video.s3.amazonaws.com/video_upload/post/217893105/c63d4f50-ca5f-459a-b368-281f73e3765e/transcoded-1790641303.png)
저희는 2주 후에 열리는 AI Engineer New York에서 Anthropic이 최신 AI x Finance 작업을 공유하게 되어 기쁩니다!
[지금 듣기](https://www.latent.space/p/thariq)> 2026년 9월 26일~9월 28일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터 계정을 확인했으며, 추가 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 호를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션임을 알려드립니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
주요 소식: Claude Sonnet 5.5 출시 및 반응

## 무슨 일이 있었나요
Anthropic은 Opus 5.5 출시 일주일 후이자 OpenAI DevDay 전날, Claude 5.5 제품군의 두 번째 모델인 Claude Sonnet 5.5를 출시했습니다. 초기 독립 평가에서는 여러 리더보드에서 Opus 5.5와 비슷하거나 그에 준하는 성능을 보였습니다.
- 출시 시점: 출시 전부터 이야기가 나왔습니다. @kimmonismus는 이미 자신의 계정으로 라우팅되고 있다고 보고했으며, @scaling01은 공식 게시물 이전에 Anthropic API에서 이를 발견했습니다.
- 공식 발표: @claudeai (53K 참여도)와 @AnthropicAI는 이를 "Sonnet 5에 대한 확실한 업그레이드"라고 불렀습니다. 이들은 대부분의 작업에서 30% 이상 더 빠르고 최대 30% 더 저렴하다고 주장합니다.
- 포지셔닝: @ClaudeDevs는 이를 "버그 수정 및 기능에 대한 빠른 반복과 같은 잘 정의된 일상적인 작업"에 적합하다고 포지셔닝합니다. Anthropic은 또한 Sonnet과 Opus 5.5 중 언제 선택할지, Sonnet 5에서 마이그레이션하는 방법, 그리고 튜닝 노력에 대한 빌드 가이드를 발행했습니다.
- 무료 티어: @simonw는 Sonnet 5.5가 이제 claude.ai의 무료 티어를 구동한다고 지적합니다. ChatGPT의 무료 티어는 여전히 GPT-5.6 Luna이며, 그는 이를 "훨씬 덜 유능하다"고 말합니다.
- 디스틸레이션 방지 변경: @ClaudeDevs는 계정 전환을 통한 디스틸레이션에 대응하기 위해 "보존된 사고(preserved thinking)"를 확장했습니다. 추론 흔적은 이를 생성한 조직에 남아 있습니다. 세션이 다른 계정으로 이동하면 Claude는 이를 다시 읽고 사고를 재생성합니다.
- 로드맵: @mikeyk는 Haiku 5.5가 "앞으로 몇 주 안에 제품군을 완성할 것"이라고 말했습니다.
- 가용성: Claude Platform과 Claude Code에 출시 당일부터 제공되었으며, 10월 22일까지 유효한 사용량 초기화가 함께 제공됩니다 (@ClaudeDevs). 서드파티 가용성:VS Code의 GitHub Copilot (@code)CursorFactoryDevin Desktop/CLIClineWebDev, Text, Vision 및 Document용 Arena Agent/Battle 모드 (@arena)T3 Code, @theo가 아직 카탈로그에 추가되지 않았음을 인정한 후

## 기술 세부 정보 및 사양

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-amd-buys-world-labs-for-82b&utm_source=paywall-free-trial&utm_medium=web&utm_content=217942537&coupon=5fe099d9)
[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-amd-buys-world-labs-for-82b&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
