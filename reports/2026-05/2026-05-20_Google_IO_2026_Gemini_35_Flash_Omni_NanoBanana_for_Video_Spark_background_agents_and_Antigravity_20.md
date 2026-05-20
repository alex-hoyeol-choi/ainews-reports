# Google I/O 2026: Gemini 3.5 Flash, Omni (NanoBanana for Video), Spark (background agents), and Antigravity 2.0

**원문 URL**: https://www.latent.space/p/ainews-google-io-2026-gemini-35-flash
**번역일**: 2026-05-20 06:20
**발행일**: 2026-05-20

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Google I/O 2026: Gemini 3.5 Flash, Omni (영상용 NanoBanana), Spark (백그라운드 에이전트), Antigravity 2.0

### Google이 바쁘게 움직였습니다!
전체 키노트 라이브스트림은 2시간이었지만, 늘 그렇듯이 The Verge가 30분으로 압축한 최고의 요약본을 제공했으며, 이는 전체적인 흐름을 파악하는 데 매우 유용합니다:
메인라인 Gemini 3.5 Flash는 오늘 GA(General Availability)되었습니다(일부 단계별 출시와 비교하면 매우 좋습니다). 이 모델은 3.1 Pro와 비교해도 상당한 개선을 이루었으며, 3.5 Pro는 다음 달에 출시될 예정입니다. 아마도 더 인상적이었던 것은 Gemini Live (음성)와 Omni (영상), 그리고 Google Pics/Flow (이미지/VFX/음악) 모달리티였는데, Google은 업계 최고 수준의 하드웨어와 모델 덕분에 업계 최고 수준의 기능과 레이턴시를 선보였습니다.
요즘 모든 빅테크 키노트의 오랜 전통에 따라, Google은 스마트 글래스 기술도 선보였는데, 이는 Google과 경쟁사들의 이전 버전들보다 길거리에서 더 많이 볼 수 있을 것 같습니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/904f7a4e-f945-40e0-b980-024fc220d0b7_1524x912.png)
> 2026년 5월 18일-5월 19일 AI 뉴스입니다. 저희는 12개의 서브레딧과 544개의 트위터를 확인했으며, 추가적인 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
Google은 I/O를 통해 Gemini를 소비자 AI 서비스이자 개발자/에이전트 플랫폼으로 재포지셔닝했으며, 세 가지 핵심 기술 발표를 했습니다: 빠른 에이전틱/코딩 워크로드용 Gemini 3.5 Flash, 영상부터 시작하는 멀티모달 생성/편집용 Gemini Omni, 그리고 데스크톱/CLI/SDK/API를 아우르는 광범위한 Antigravity 에이전트 스택입니다. 공식 게시물들은 스케일을 강조했습니다 — Google은 현재 월 3.2 경(quadrillion) 토큰 이상을 처리하며, 이는 전년 대비 월 480조(trillion) 토큰에서 7배 증가한 수치라고 밝혔습니다. 또한 Gemini 앱은 월 9억 명 이상의 사용자를 보유하고 있으며 230개 이상의 국가와 70개 이상의 언어로 제공됩니다 (Google, Google, GeminiApp). 가장 기술적으로 중요한 출시는 Gemini 3.5 Flash였으며, Google은 이를 자사의 가장 강력한 에이전틱/코딩 모델로 소개했습니다. 이 모델은 즉시 GA되었으며, 1M 토큰 컨텍스트, 65k 최대 출력, 4단계 사고 레벨("minimal/low/medium/high"), 그리고 여러 턴에 걸친 "thought preservation" 기능을 제공합니다 (GoogleDeepMind, Google, _philschmid). Google은 Gemini 추론과 생성형 미디어를 결합한 새로운 제품군인 Gemini Omni를 함께 발표했습니다. Omni Flash를 통해 텍스트/이미지/영상/오디오 입력을 받아 Gemini, Flow, Shorts에서 영상 편집/생성을 수행하며, 추후 API로도 제공될 예정입니다 (GoogleDeepMind, Google, GeminiApp). 이러한 모델들을 중심으로 Google은 Antigravity 2.0 데스크톱, CLI, SDK, Gemini API의 Managed Agents, Search-native 생성형 UI/코딩, 클라우드 VM의 Gemini Spark 백그라운드 에이전트, 그리고 Gemini 앱/Workspace/commerce/media 통합의 긴 목록을 출시하거나 확장했습니다 (Google, Google, Google).

## 사실 vs. 의견

### 사실 / 공식 또는 서드파티 벤치마크 소스에서 직접 주장한 내용
- Google은 현재 월 3.2 경(quadrillion) 토큰을 처리하며, 이는 1년 전 월 480조(trillion) 토큰에서 증가한 수치라고 밝혔습니다 (Google).
- Google은 Gemini가 월 9억 명 이상의 사용자를 보유하고 있다고 밝혔습니다 (Google).
- Google은 Gemini 3.5 Flash가 오늘 Gemini 앱, Search AI Mode, Gemini API, AI Studio, Antigravity, Android Studio 및 엔터프라이즈 서비스 전반에 걸쳐 GA되었다고 밝혔습니다 (Google, GeminiApp).
- Google은 Gemini 3.5 Flash가 1M 컨텍스트, 65k 최대 출력, 4단계 사고 레벨, 그리고 여러 턴에 걸친 "thought preservation" 기능을 제공한다고 밝혔습니다 ( _philschmid).
- Google은 3.5 Flash가 Terminal-Bench 2.1, GDPval-AA, MCP Atlas에서 Gemini 3.1 Pro를 능가한다고 밝혔습니다 (GoogleDeepMind, Google).
- Google은 3.5 Flash가 유사한 프론티어 모델보다 4배 빠르며, Antigravity에서는 최대 12배 빠르다고 밝혔습니다 (Google, JeffDean).
- 독립 벤치마커 Artificial Analysis는 Gemini 3.5 Flash가 Intelligence Index에서 55점을 기록하여 Gemini 3 Flash보다 +9점 높고, >280 output tok/s를 달성했으며, MMMU-Pro 84%, GDPval-AA Elo 1656, 그리고 1M 입력/출력 토큰당 $1.50 / $9.00의 가격을 가진다고 보고했습니다. 또한 이 모델이 자사 스위트에서 Gemini 3 Flash보다 5.5배, Gemini 3.1 Pro보다 75% 더 비싸다고 보고했습니다 (ArtificialAnlys).
- Arena는 Gemini 3.5 Flash가 Text Arena 전체에서 #9위, Code Arena: Frontend에서 #9위를 기록했으며, 1507점으로 Gemini 3 Flash보다 +70점 상승하여 해당 가격대에서 최고 점수를 달성했다고 보고했습니다 (arena).
- Google은 Gemini Omni Flash가 오늘부터 유료 사용자에게 Gemini/Flow에서 제공되며, 이번 주부터 Shorts/Create에서 무료로 제공되고, 몇 주 내로 API를 통해 제공될 예정이라고 밝혔습니다 (Google).
- Google은 Spark가 전용 Google Cloud 가상 머신에서 실행되어 사용자 장치가 꺼져 있어도 장시간 실행되는 작업을 허용한다고 밝혔습니다 (Google).
- Google은 Antigravity + Gemini 3.5 Flash 데모가 93개의 병렬 서브 에이전트, 15k개 이상의 모델 요청, 2.6B 토큰, 그리고 $1K 미만의 API 크레딧을 사용하여 12시간 만에 작동하는 OS를 구축했다고 주장했습니다 (Google).
- Google은 Search가 Antigravity + 3.5 Flash를 사용하여 즉석에서 맞춤형 시각 도구/시뮬레이션을 생성할 것이라고 밝혔습니다 (Google).

### 의견 / 해석 / 회의론
- 긍정적인 평가: "Google이 돌아왔다", "Flash 모델치고는 미친 듯한 평가", "AGI를 향한 세계 모델", Search + Antigravity에 대해 "놀랍다" 등 (kimmonismus, Kseniase_, demishassabis).
- 중립적인 주의: 일부 게시자들은 자체 보고된 벤치마크 때문에 과대평가를 명시적으로 피했으며, 가격/성능 문제를 언급했습니다 (scaling01, simonw).
- 부정적/회의적인 평가:
    *   이전 Flash 모델 대비 가격 인상 (enricoros).
    *   GPT-5.5-medium이 엔드투엔드에서 더 스마트하고/저렴하고/빠를 수 있다는 비교 (scaling01, scaling01).
    *   약한 TerminalBench-Hard, 평범한 MRCR / ARC-AGI-2, 또는 일부 영역에서 Kimi/GLM을 명확히 능가하지 못하는 등 벤치마크의 한계 (scaling01, teortaxesTex, scaling01).
    *   Gemini CLI와 Antigravity CLI 사이의 제품명/UX 혼란 및 전반적인 인터페이스 디자인 비판 (zachtratar, kchonyc, teortaxesTex).

## Gemini 3.5 Flash: 주요 기술 출시

### 공식 포지셔닝
Google/DeepMind는 Gemini 3.5 Flash를 자사의 절대적인 플래그십 인텔리전스 모델이 아닌, 에이전트 및 코딩을 위한 가장 강력한 모델로 반복해서 설명했습니다. 이 모델은 Google 제품과 개발자 워크로드 모두를 지원하며, 파레토 프론티어의 고속, 고유틸리티 부분에 위치하도록 설계되었습니다 (GoogleDeepMind, Google, SundarPichai).

### 기술 세부 사항 및 지표
Google 및 관련 게시물에서 발췌:
- GA(General Availability) 즉시 가능 (Google)
- 1M 토큰 컨텍스트 윈도우
- 65k 최대 출력 토큰
- 사고 레벨: minimal, low, medium (새로운 기본값), high
- 다중 턴 대화 전반에 걸친 thought preservation
- 텍스트 출력
- 입력 모달리티: Artificial Analysis에 따르면 텍스트, 이미지, 영상, 음성 ( _philschmid, ArtificialAnlys)
- 가격: 1M 입력 토큰당 $1.50, 1M 출력 토큰당 $9.00, 캐시된 입력에 90% 할인 (scaling01, ArtificialAnlys)
공식 벤치마크 주장:
- Terminal-Bench 2.1: 76.2%
- GDPval-AA: 1656 Elo
- MCP Atlas: 83.6%
- Google이 인용한 멀티모달 결과: 한 엔지니어 게시물에서 MMMU-Pro 83.6%; Artificial Analysis는 자사 설정에서 기록된 최고치인 84%를 보고했습니다 (koraykv, ArtificialAnlys)
속도 주장:
- Google 마케팅 주장: 유사한 프론티어 모델보다 4배 빠름 (Google)
- Antigravity에서는 Google이 최대 12배 빠르다고 밝혔습니다 (JeffDean, scaling01)
- Artificial Analysis는 >280 output tok/s를 관찰했습니다
- 일부 논의에서는 Antigravity에 특화된 최적화된 서빙에서 약 867 tok/s를 언급했습니다 (scaling01, scaling01)
서드파티 평가:
- Artificial Analysis는 3.5 Flash가 지능-대-속도 파레토 프론티어에서 선두 주자이지만, 경제성은 이전 Flash보다 현저히 나쁘다고 말합니다:
    *   Intelligence Index에서 Gemini 3 Flash보다 55+9점
    *   환각(Hallucination)률이 61%로 감소, Gemini 3 Flash 대비 자사 omniscience 설정에서 31%p 하락
    *   GDPval-AA 1656 Elo
    *   자사 벤치마크 스위트에서 Gemini 3 Flash보다 5.5배 더 비쌈
    *   동일 스위트에서 Gemini 3.1 Pro보다 75% 더 비쌈 (ArtificialAnlys)
Arena:
- #9 Text Arena
- #9 Code Arena: Frontend
- 1507점, Gemini-3 Flash 대비 +70점
- 프론트엔드 코딩 평가에서 Gemini 3.1 Pro를 모든 카테고리에서 능가 (arena, arena)

### 시사점
주목할 만한 변화는 Google이 이전 주기에서는 배포에 최적화된 하이엔드 제품 모델처럼 설명되었을 모델에 "Flash"라는 라벨을 사용하고 있다는 점입니다. 이는 단순히 저렴한 경량 티어가 아닙니다. 여러 게시자들이 이 점을 직접 지적하며, Flash가 더 비싸지고 있으며 이전 Pro 영역을 흡수하고 있을 수 있다고 주장했습니다 (enricoros, simonw).
가장 강력한 기술적 신호는 "최고의 절대 벤치마크 모델"이 아니라 다음입니다:
1.  실질적인 에이전틱 성능 향상
2.  극도로 빠른 서빙 속도
3.  제품 서비스에 대한 깊은 통합
4.  서브 에이전트 및 장기 실행을 중심으로 구축된 툴링
이러한 점들로 인해 3.5 Flash는 일부 경쟁자들이 특정 서드파티 비교에서 순수 가격 조정 지능에서 여전히 우위를 점하더라도 전략적으로 중요합니다.

## Gemini Omni: "어떤 입력으로든 무엇이든 생성"하는 멀티모달 생성/편집

### Google이 발표한 내용
Google은 Gemini 추론/세계 지식과 Google의 생성형 미디어 스택을 결합한 새로운 제품군으로 Gemini Omni를 소개했으며, 영상 생성 및 편집부터 시작합니다. 공식 메시지는 이를 "어떤 입력으로든 무엇이든 생성"한다고 설명했지만, 현재 출시는 더 좁습니다:
- 입력: 텍스트, 이미지, 오디오, 영상
- 초기 출력 강조: 영상
- 제품 가용성: Gemini 앱, Flow, YouTube Shorts/Create, 추후 API
- 현재 출시 모델: Gemini Omni Flash (GoogleDeepMind, Google, Google)
Google/DeepMind의 주장:
- 더 나은 세계 이해
- 더 견고한 물리
- 장면/캐릭터 일관성이 유지되는 다중 턴 편집
- 대화형 편집으로 사용자 영상 푸티지를 "재해석"하는 능력 (Google, Google)
출시 세부 사항:
- 유료 Gemini 사용자에게 앱/Flow에서 전 세계적으로 "오늘"부터 제공
- YouTube Shorts/Create는 "이번 주부터" 무료로 출시 예정
- 개발자/엔터프라이즈용 API는 몇 주 내로 제공 예정 (Google, GeminiApp)

### 관점
- 지지: 사용자들과 Google 직원들은 Omni를 특히 영상 편집 및 일관성 측면에서 주요한 품질 개선 단계로 평가했습니다 (joshwoodward, fofrAI, osanseviero).
- 전략적 해석: 여러 게시자들은 Omni를 Google이 텍스트/코드 경쟁뿐만 아니라 세계 모델 및 체화된/물리적 사전 지식에 투자하고 있다는 증거로 보았습니다 (demishassabis, jparkerholder, kimmonismus).
- 회의론: 일부 UI/출력 예시는 "B급 비디오 게임 인터페이스" 같거나 너무 세련되고 템플릿 같다는 비판을 받았습니다 (teortaxesTex, shlomifruchter).

### 맥락
Omni는 "또 다른 영상 모델"로서의 의미보다는 Google이 다음을 통합하려는 시도로서 더 중요합니다:
- 멀티모달 이해
- 미디어 편집
- 세계 기반 다지기(world grounding)
- 에이전트 인터페이스
- 그리고 궁극적으로 모든 입력/모든 출력 생성
이는 DeepMind의 오랜 세계 모델 의제와 Google의 제품 배포 이점과 일치합니다.

## Antigravity: Google의 에이전트 OS, 단순한 코딩 어시스턴트가 아닙니다
I/O에서 크게 저평가되었던 주제 중 하나는 Google이 더 이상 에이전트를 챗 모델을 감싸는 얇은 래퍼로 제시하지 않는다는 점입니다. Antigravity는 실행 기반(execution substrate)이 되고 있습니다.

### 출시/확장된 내용
- Antigravity 2.0 데스크톱 앱: 핵심 대화, 아티팩트, 다중 에이전트 오케스트레이션을 갖춘 에이전트 우선 데스크톱 (Google, Google)
- Antigravity CLI (Google, Google)
- Antigravity SDK (Google)
- Gemini API의 Managed Agents: 단일 API 호출로 에이전트와 호스팅된 Linux 샌드박스를 제공합니다. Bash/Python/Node, 파일, 브라우징, 커스텀 마크다운 정의 스킬, repo/GCS 마운트를 지원합니다 (Google, GoogleAIStudio, _philschmid)
- AI Studio, Android, Firebase, Workspace, 웹과의 통합 (Google, Google)
- AI Studio에서 Antigravity로 원클릭 내보내기 (Google)
- AI Studio의 네이티브 Android 앱 생성 / Antigravity의 Android 지원 (Google, AndroidDev)

### 기술적 신호
Google 자체 데모는 병렬 서브 에이전트, 호스팅된 실행, 고주파 반복 루프, 아티팩트 중심 워크플로우에 중점을 두었습니다. Jeff Dean은 3.5 Flash를 "협업하고, 고주파 반복 루프를 실행하며, 실제 문제를 대규모로 해결하는 서브 에이전트를 배포"하기 위한 강력한 엔진으로 명시적으로 설명했습니다 (JeffDean).
주요 증거:
- 12시간 만에 구축된 OS
- 93개의 병렬 서브 에이전트
- 15k개 이상의 요청
- 2.6B 토큰
- $1K 미만의 크레딧 (Google)
이것이 대부분 연출된 벤치마크/데모라고 할지라도, Google이 개발자들이 채택하기를 원하는 아키텍처를 보여줍니다: 느린 하나의 모놀리식 실행보다는 많은 빠른 에이전트.

### 반응
- 긍정적: 이는 Google이 Codex/Claude Code/OpenClaw/Hermes 스타일 워크플로우에 대한 답변이며, 더 강력한 인프라 스토리를 가지고 있습니다 (iScienceLuvr, theo).
- 비판적: 브랜딩과 제품 확산은 여전히 혼란스럽습니다. 일부 사용자들은 Gemini CLI를 사용해야 할지 Antigravity CLI를 사용해야 할지 확신하지 못하며, Google의 디자인 선택은 불만을 야기했습니다 (kchonyc, zachtratar, teortaxesTex).

## Search, Gemini 앱, 그리고 소비자 에이전트

### Search
Google은 재설계된 AI 기반 Search 박스, 멀티모달 쿼리 지원, 그리고 가장 야심 찬 소비자 대상 움직임을 발표했습니다: Antigravity + Gemini 3.5 Flash를 사용하여 즉석에서 맞춤형 시각 도구 및 시뮬레이션을 생성하는 Search입니다 (Google, Google).
또한 Search 내 정보 에이전트를 미리 선보였습니다:
- 지속적인 모니터링 작업
- 웹/뉴스/소셜/실시간 신호
- 링크 및 작업이 포함된 종합 업데이트
- 이번 여름 Pro/Ultra 사용자에게 출시 예정 (Google, Google)
이는 주목할 만한 전략적 변화입니다: Search는 리트리벌/랭킹에서 백그라운드 에이전틱 모니터링 + 생성된 애플릿으로 전환합니다.

### Gemini 앱
소비자 Gemini 업데이트에는 다음이 포함됩니다:
- 새로운 "Neural Expressive" 디자인 언어 (Google)
- 인라인/즉시 Gemini Live 음성 (Google)
- 받은 편지함/캘린더/작업에서 개인화된 Daily Brief 요약 (Google, GeminiApp)
- 클라우드 VM에서 24시간 내내 작동하며 주요 작업 전에 사용자에게 확인하는 개인 AI 에이전트인 Gemini Spark (Google, GeminiApp)
- macOS 앱 + 곧 출시될 Spark/음성 데스크톱 워크플로우 (Google, GeminiApp)

### 가격 / 구독
Google은 새로운 가격 체계를 도입했습니다:
- 새로운 월 $100 요금제
- 최고 티어 Ultra는 월 $250에서 $200로 인하 (Google, GeminiApp)
이는 프리미엄 파워 유저, 특히 코더와 크리에이터를 위한 보다 공격적인 입찰로 해석됩니다.

## 신뢰, 출처(provenance), 그리고 표준
Google은 Search, Gemini, Chrome, 하드웨어/미디어 서비스 전반에 걸쳐 SynthID를 추진했으며, OpenAI, NVIDIA, Kakao, ElevenLabs와의 파트너십을 발표하여 이들의 생성된 콘텐츠에 SynthID를 적용할 예정입니다 (Google, Google).
이는 I/O에서 발표된 더 중요한 표준 관련 움직임 중 하나입니다:
- 이는 Google에게 생성형 미디어의 출처(provenance) 레이어 일부를 소유할 기회를 제공합니다.
- 특히, OpenAI는 SynthID 워터마크 + C2PA 자격 증명을 통해 OpenAI가 생성한 이미지를 확인하는 지원을 별도로 발표했습니다 (OpenAI).
이것은 Omni/3.5 Flash보다 덜 화려했지만, 출처(provenance)가 필수 인프라가 된다면 더 오래 지속될 가능성이 높습니다.

## Google의 과학 및 세계 모델 관점
여러 I/O 항목들은 Google이 코딩/챗 분야에서만 경쟁하고 싶어 하지 않는다는 점을 강조했습니다:
- Gemini for Science: Literature Insights, Hypothesis Generation, Computational Discovery (GoogleDeepMind, Google)
- ERA / Co-Scientist 관련 Nature 출판 링크 (GoogleResearch, GoogleResearch)
- Project Genie + Street View 기반 다지기(grounding), 약 20년간의 지도 이미지를 사용하여 인터랙티브한 실제 위치 시뮬레이션 생성 (Google, poolio, bilawalsidhu)
이러한 광범위한 맥락은 일부 관찰자들이 Omni를 단순한 콘텐츠 도구가 아닌 "세계 모델 발전"으로 해석한 이유를 설명합니다 (demishassabis, jparkerholder).

## 다양한 의견

### 낙관적 / 지지적
- Gemini 3.5 Flash는 특히 에이전틱 코딩 분야에서 속도 티어 모델로서 큰 도약으로 평가됩니다 (kimmonismus, SundarPichai).
- Search + Antigravity는 Google이 생성된 UI/도구를 엄청난 규모로 배포할 수 있기 때문에 잠재적으로 혁신적이라고 여겨집니다 (Kseniase_, TheTuringPost).
- Omni는 편집 품질과 더 깊은 세계 모델 로드맵을 암시한다는 점에서 칭찬받았습니다 (joshwoodward, kimmonismus).

### 회의적 / 반대적
- Google이 자체 보고된 벤치마크에 의존하고 있으며, 독립적인 비교에서는 여전히 경쟁사들이 우위를 점할 여지가 있다는 우려 (scaling01).
- "Flash"라는 이름이 더 이상 저렴하다는 것을 정당화할 만큼 충분히 싸지 않다는 우려; 가격이 이전 Flash 세대보다 급격히 상승했습니다 (enricoros, simonw).
- 일부는 GPT-5.5-medium이 스마트함/저렴함/레이턴시를 종합적으로 고려할 때 여전히 우세하다고 믿었습니다 (scaling01).
- 일부 벤치마크 영역에서는 불균형이 있음을 시사합니다 — 예를 들어, 강력한 에이전틱 수치에도 불구하고 TerminalBench-Hard의 성능이 좋지 않거나 추론 지표가 평범하다는 점 (scaling01, teortaxesTex).

### 중립적 / 분석적
- Artificial Analysis는 가장 강력하고 균형 잡힌 평가를 내렸습니다: 뛰어난 속도-지능 프론티어 위치, 상당한 에이전틱 성능 향상, 그러나 이전 Flash보다 실질적으로 나쁜 비용 효율성, 심지어 자사의 엔드투엔드 스위트에서는 3.1 Pro보다도 높습니다 (ArtificialAnlys).
- Arena의 데이터 또한 특히 프론트엔드/코드 작업에서 "단순한 마케팅이 아닌 실제 개선"이라는 결론을 지지하며, 카테고리 지배를 주장하지는 않습니다 (arena).

## 왜 이것이 중요한가
1.  Google은 이제 일관된 배포 스토리를 가지고 있습니다.
    이전 Gemini 주기들은 종종 벤치마크 중심적이고 제품이 파편화된 느낌을 주었습니다. I/O에서 Google은 모델, 인프라, 도구, API, 소비자 서비스, 그리고 엔터프라이즈 출시를 하나로 묶었습니다.
2.  중심축이 챗봇 UX에서 에이전트 실행으로 이동하고 있습니다.
    중요한 기본 요소는 단순히 모델 IQ가 아니었습니다: 서브 에이전트, 호스팅된 샌드박스, 장기 실행 작업, 생성된 아티팩트, 그리고 Search/Workspace/Android와의 통합이었습니다.
3.  Gemini 3.5 Flash는 "많은 에이전트를 오케스트레이션할 만큼 충분히 빠름"이 최대 벤치마크 점수보다 더 중요할 수 있음을 시사합니다.
    코딩 및 도구 사용의 경우, 처리량(throughput)과 레이턴시(latency)는 점점 더 제품을 정의하는 요소가 되고 있습니다.
4.  Omni는 Google의 차별화 전략을 보여줍니다.
    Google은 순전히 텍스트 중심의 경쟁보다는 멀티모달/세계 기반(world-grounded) 시스템에 베팅하고 있습니다.
5.  신뢰/출처(provenance)가 플랫폼 인프라가 되고 있습니다.
    OpenAI/NVIDIA/ElevenLabs/Kakao와의 SynthID 파트너십은 콘텐츠 인증 출처(provenance) 레이어 주변에서 일부 수렴이 이루어지고 있음을 시사합니다.
6.  가장 큰 미해결 과제는 경제성입니다.
    기술적으로 강력하든 아니든, 3.5 Flash는 비용 인상에 대한 상당한 반발을 불러일으켰습니다. 만약 "Flash"가 더 이상 저렴한 주력 티어가 아니라면, Google은 기능 배포에서는 승리할 수 있지만 예측 가능성과 가격 단순성 측면에서 일부 개발자들의 마음을 잃을 수 있습니다.
인재, 연구소, 그리고 생태계 움직임
- Karpathy, Anthropic 합류: 그날 가장 많이 언급된 AI 트윗은 Andrej Karpathy가 "R&D로 돌아가기 위해" Anthropic에 합류했다고 발표한 것이었습니다. 이 트윗은 논의를 지배했으며, @scaling01은 Axios를 인용하여 그가 RSI/autoresearch에 참여하고 새로운 사전 학습(pretraining) 중심 노력을 시작할 것이라는 추측을 내놓았습니다. 세부 사항은 Anthropic에 의해 확인되지 않았지만, 이 움직임은 Anthropic에게 주요한 인재 영입 승리로 널리 해석되었습니다.
- OpenAI 용량 제품: OpenAI는 고객이 중요한 워크로드를 위해 장기적인 컴퓨팅 액세스를 확보할 수 있도록 하는 상업적 제안인 Guaranteed Capacity를 발표했습니다. Sam Altman은 모델이 더욱 유용해짐에 따라 용량 제약이 계속될 세상에 대한 대응으로 이를 설명하며, 1~3년 약정에 대해 할인된 토큰을 제공한다고 밝혔습니다.
- GitHub 및 코딩 툴체인 통합: GitHub는 Gemini 3.5 Flash가 Copilot에 출시되고 있다고 밝히며, 반복적인 에이전틱 코딩을 위한 강력한 도구 사용, 빠른 응답 시간, 캐시 효율성을 언급했습니다. Cursor는 Jira와의 통합을 출시하여 클라우드 에이전트가 작업 항목을 가져와 병합 준비된 PR을 생성할 수 있도록 했습니다. Code/VS Code 또한 Gemini 3.5 Flash 가용성을 발표했습니다.
학습 알고리즘, 벤치마크, 그리고 에이전트 평가
- RL/사후 학습(post-training) 논의가 더 밀도 높은 크레딧 할당으로 전환 중: @nrehiew_는 다음 확장 가능한 학습 돌파구가 GRPO를 기반으로 하되, ECHO, Composer2, self-distillation, OPD와 같은 방향을 인용하며 더 밀도 높고 편향이 낮은 크레딧 할당을 통해 구축될 수 있다고 주장했습니다. @lateinteraction은 "교육적 RL" 프레이밍으로 반박했습니다: 올바르고 따라하기 쉬운 롤아웃을 샘플링하는 자기 교사를 학습시키는 것입니다.
- 코딩 에이전트가 연구를 할 수 있을까? 아직은 아닙니다: Intology AI는 NanoGPT Speedrun 경쟁을 기반으로 한 자율 벤치마크인 NanoGPT-Bench를 출시하여 코딩 에이전트가 실제 AI R&D 발전에 기여할 수 있는지 테스트했습니다. 그들의 주요 결과: Codex, Claude Code, Autoresearch는 인간 발전의 9.3%만을 회복했으며, 이는 알고리즘 혁신보다는 주로 하이퍼파라미터 튜닝을 통한 것이었습니다.
- 에이전트 하네스 및 메모리가 더욱 공식화되고 있습니다: @omarsar0은 코드-as-에이전트-하네스에 대한 100페이지 이상의 설문조사를 강조하며, 미래 시스템은 실행 가능하고, 검사 가능하며, 상태를 유지하고, 통제되어야 한다고 주장했습니다. François Chollet은 실제 작업은 마르코프적이지 않은 경우가 거의 없으므로, 고충실도 궤적 압축이 없는 에이전트는 극적으로 덜 유용하다는 관련 요점을 지적했습니다.
- 검증자(Verifier) 품질이 병목 현상으로 부상: @Shahules786의 스레드는 에이전트 벤치마크를 확장하는 것이 이제 작업 추가보다는 검증자 품질 향상에 더 많이 의존한다고 강조하며, SWE-bench Verified, OSWorld-Verified, ComputerRL, BenchGuard를 인용했습니다.
과학, 생물학 모델, 그리고 도메인 특화 시스템
- Hugging Face, Carbon DNA 모델 출시: 가장 기술적으로 흥미로운 오픈 릴리스 중 하나는 생성형 DNA 파운데이션 모델 제품군인 Carbon이었습니다. 팀은 Carbon-3B가 Evo2-7B와 일치하면서 인퍼런스 속도가 250-275배 더 빠르며, 단일 GPU에서 이틀 이내에 전체 인간 게놈을 처리하기에 충분하다고 말합니다. 주요 레시피 변경 사항: 결정론적 6-mer 토큰화, 학습 후반에 일반 교차 엔트로피를 대체하는 인자화된 손실(FNS), 그리고 @LoubnaBenAllal1에 따른 기능성 DNA + mRNA 데이터의 선별된 단계별 혼합입니다. 이 릴리스에는 모델, 학습 코드, 평가, 데이터 및 데모가 포함됩니다.
- Google, AI for science를 제품 카테고리로 추진: Google은 연구자들을 위한 프로토타입 스위트인 Gemini for Science를 소개했습니다: Literature Insights (NotebookLM을 통한 논문 합성), Hypothesis Generation (Co-Scientist 스타일의 다중 에이전트 "아이디어 토너먼트"), 그리고 Computational Discovery (AlphaEvolve 및 ERA로 구축되어 수천 개의 코드 변형을 병렬로 생성하고 점수를 매김). Google Research는 또한 ERA가 Nature에 출판되었다고 언급했습니다 (Google Research).
- 특화된 사전 학습(pretraining)이 지지를 얻고 있습니다: @pratyushmaini는 초기 노출/특화된 사전 학습(pretraining)이 망각에 대한 견고성을 향상시킨다는 증거를 지적하며, 도메인 사용 사례에 진지한 기업들은 사후 학습(post-training)뿐만 아니라 처음부터 맞춤형 모델을 학습시키는 것을 고려해야 한다고 주장했습니다.
내부 에이전트의 안전성, 거버넌스 및 모니터링
- METR의 첫 번째 프론티어 리스크 보고서: METR은 Anthropic, Google, Meta, OpenAI 전반에 걸친 이례적으로 깊은 접근을 기반으로 한 주요 새 보고서를 발표했으며, 모델 CoT 및 기능, 정렬, 제어에 대한 비공개 정보를 포함합니다. 이 보고서는 연구소들이 자체적으로 배포한 내부 AI 에이전트에 대한 통제력을 잃을 수 있는지에 초점을 맞추고 있으며, 광범위한 부록과 기록을 포함합니다 (METR).
- 내부 에이전트 모니터링은 이제 활발한 관행입니다: @idavidrein은 Anthropic에 한 달 동안 상주하며 내부 AI 에이전트가 "폭주"할 수 있는지 감지하도록 설계된 시스템을 스트레스 테스트했다고 설명했습니다. 그가 언급한 주요 주의사항은 이 연습이 Anthropic에게 민감한 정보를 수정할 재량권을 허용했으므로, 그는 이를 공식 감사라기보다는 연습으로 간주한다는 것입니다.
- 새로운 안전 표준 조직: Steven Adler는 Page Hedley와 공동 설립한 새로운 AI 안전 표준 조직인 Guidelight를 발표하며 첫 두 가지 표준을 공개했습니다. 데이터셋의 트윗 스레드는 부분적이지만, 이 움직임은 모델 평가뿐만 아니라 운영 표준을 중심으로 분야가 전문화되고 있다는 또 다른 신호로서 주목할 만합니다.
가장 많이 언급된 트윗 (참여도 기준)
- Karpathy, Anthropic 합류: @karpathy
- Google, Gemini 3.5 모델 시리즈 소개: @Google
- Google DeepMind, Gemini Omni 출시: @GoogleDeepMind
- 에이전트 및 코딩용 Gemini 3.5 Flash GA: @Google
- OpenAI Guaranteed Capacity: @OpenAI
- Google의 24시간 개인 에이전트, Gemini Spark: @Google

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

## 7일 무료 체험으로 계속 읽으세요
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일 동안 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-google-io-2026-gemini-35-flash&utm_source=paywall-free-trial&utm_medium=web&utm_content=198494270&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-google-io-2026-gemini-35-flash&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
