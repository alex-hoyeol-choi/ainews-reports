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
| 2026-02-28 | OpenAI closes $110B raise from Amazon, NVIDIA, SoftBank in largest startup fundraise in history @ $840B post-money | [전체번역](reports/2026-02/2026-02-28_OpenAI_closes_110B_raise_from_Amazon_NVIDIA_SoftBank_in_largest_startup_fundraise_in_history_840B_post-money.md) | [요약](reports/2026-02/2026-02-28_OpenAI_closes_110B_raise_from_Amazon_NVIDIA_SoftBank_in_largest_startup_fundraise_in_history_840B_post-money_summary.md) | [HTML](reports/2026-02/2026-02-28_OpenAI_closes_110B_raise_from_Amazon_NVIDIA_SoftBank_in_largest_startup_fundraise_in_history_840B_post-money_summary.html) |
2026-02-25 | Agentic Engineering: WTF Happened in December 2025? | [전체번역](reports/2026-02/2026-02-25_Agentic_Engineering_WTF_Happened_in_December_2025.md) | [요약](reports/2026-02/2026-02-25_Agentic_Engineering_WTF_Happened_in_December_2025_summary.md) | [HTML](reports/2026-02/2026-02-25_Agentic_Engineering_WTF_Happened_in_December_2025_summary.html) |

## 자동 번역 시스템

- **번역 엔진**: Google Gemini 3.1 Pro (기본) / OpenAI GPT (백업)
- **모니터링**: 6시간 간격 자동 체크
- **소스 코드**: [ainews](https://github.com/alex-hoyeol-choi/ainews)

---

*이 리포지토리의 콘텐츠는 자동 생성된 번역입니다.*
