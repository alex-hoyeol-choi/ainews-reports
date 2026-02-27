# ainews-reports

AI 뉴스레터 한국어 번역 아카이브

[ainews](https://buttondown.com/ainews) 및 [news.smol.ai](https://news.smol.ai) 뉴스레터를 자동으로 한국어 번역·요약하여 보관합니다.

## 구조

```
reports/
├── ainews/                # ainews 뉴스레터 번역
│   └── YYYYMMDD_*.md
└── smolai/                # news.smol.ai 뉴스레터 번역
    └── YYYY-MM/
        ├── *slug*.md              # 전체 번역
        ├── *slug*_summary.md      # 요약 (Markdown)
        └── *slug*_summary.html    # 요약 (HTML)
```

## 리포트 목록

| 날짜 | 제목 | 전체번역 | 요약 | HTML |
|------|------|----------|------|------|
| 2026-02-25 | Agentic Engineering: WTF Happened in December 2025? | [전체번역](reports/2026-02/2026-02-25_Agentic_Engineering_WTF_Happened_in_December_2025.md) | [요약](reports/2026-02/2026-02-25_Agentic_Engineering_WTF_Happened_in_December_2025_summary.md) | [HTML](reports/2026-02/2026-02-25_Agentic_Engineering_WTF_Happened_in_December_2025_summary.html) |
| 2026-02-25 | Agentic Engineering: WTF Happened in December 2025? | [전체번역](reports/2026-02/2026-02-25_Agentic_Engineering_WTF_Happened_in_December_2025.md) | [요약](reports/2026-02/2026-02-25_Agentic_Engineering_WTF_Happened_in_December_2025_summary.md) | [HTML](reports/2026-02/2026-02-25_Agentic_Engineering_WTF_Happened_in_December_2025_summary.html) |
| 2026-02-24 | Claude Code | [2026-02-24-claude-code.md](reports/smolai/2026-02/2026-02-24-claude-code.md) | [2026-02-24-claude-code_summary.md](reports/smolai/2026-02/2026-02-24-claude-code_summary.md) | [2026-02-24-claude-code_summary.html](reports/smolai/2026-02/2026-02-24-claude-code_summary.html) |
| 2026-02-24 | Anthropic accuses DeepSeek, Moonshot and MiniMax | [full](reports/ainews/Anthropic_accuses_DeepSeek_Moonshot_and_MiniMax__20260224_173248.md) | [summary](reports/ainews/Anthropic_accuses_DeepSeek_Moonshot_and_MiniMax__20260224_173248_summary.md) | [html](reports/ainews/Anthropic_accuses_DeepSeek_Moonshot_and_MiniMax__20260224_173248_summary.html) |
| 2025-10-09 | OpenAI Dev Day: Apps SDK, AgentKit, Codex GA, GPT | [full](reports/ainews/OpenAI_Dev_Day_Apps_SDK_AgentKit_Codex_GA_GPT_20251009_024455.md) | - | - |
| 2025-10-06 | Thinking Machines Tinker LoRA based LLM fine-tuning | [full](reports/ainews/Thinking_Machines_Tinker_LoRA_based_LLM_fine-tun_20251006_213109.md) | - | - |
| 2025-10-06 | Sora 2 new video/audio model and OpenAI's first S | [full](reports/ainews/Sora_2_new_videoaudio_model_and_OpenAIs_first_S_20251006_000413.md) | - | - |

## 자동 번역 시스템

- **번역 엔진**: Google Gemini 3.1 Pro (기본) / OpenAI GPT (백업)
- **모니터링**: 6시간 간격 자동 체크
- **소스 코드**: [ainews](https://github.com/alex-hoyeol-choi/ainews)

---

*이 리포지토리의 콘텐츠는 자동 생성된 번역입니다.*
