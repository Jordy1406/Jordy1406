# Jordy Dwi Prakoso — AI Quality Engineer

I test, evaluate and red-team LLM apps and AI agents before they touch real users and real money.
QA automation engineer with 5+ years in banking, payments and securities · Jakarta (UTC+7) · **open to remote roles
and project work**.

## AI quality portfolio (2026)

Everything below tests one system I built for the purpose: **[FinAssist ID](https://github.com/Jordy1406/finassist-app)**,
a Bahasa Indonesia RAG assistant over public capital-market documents, plus an agent that trades on a **mock** broker.
All numbers come from real runs and link to the evidence.

| Project | What I did | Result |
|---|---|---|
| [**ai-redteam**](https://github.com/Jordy1406/ai-redteam) | Threat model on OWASP Top 10 for LLM Applications 2026, 99 automated + 12 manual attacks, fixes, retest, [pentest-style report](https://github.com/Jordy1406/ai-redteam/blob/main/docs/REDTEAM_REPORT.md) | 11 findings (2 High); another client could confirm a user's order → fixed; manual attacks resisted **6/12 → 12/12** |
| [**agent-test-suite**](https://github.com/Jordy1406/agent-test-suite) | 15 multi-step agent scenarios run 3× with tool-call and broker-state assertions; readiness checklist | pass^3 **11/15**; wrong-but-valid orders execute after confirmation → **no-go** for real accounts |
| [**eval-platform**](https://github.com/Jordy1406/eval-platform) | Eval-as-CI: quality gate vs `main`, response cache, SQLite history, Streamlit dashboard | A "more helpful" prompt raised false refusals **36% → 64%** and was **blocked**; unchanged code re-checks in ~1 s |
| [**llm-eval-harness**](https://github.com/Jordy1406/llm-eval-harness) | Eval design, case format, deterministic + local LLM-judge metrics, DeepEval, paired bootstrap CIs | Hallucination-with-citation **20%** on 20 reviewed cases (judge uncalibrated; calibration next) |
| [**ai-app-tests**](https://github.com/Jordy1406/ai-app-tests) | API tests for non-deterministic output: schema, rules, majority vote, LLM-as-judge | 48 tests, single-run flaky rate **2.1%**, 3 bugs reported with reproductions |
| [**job-scout-agent**](https://github.com/Jordy1406/job-scout-agent) | Local agent that scores job postings: schema-validated extraction, rule readers, tracker formula | First live run failed (model returned nulls) → rules-first redesign; samples scored correctly |

Built with: Python · pytest · FastAPI · Ollama · Docker · promptfoo · DeepEval · Streamlit · httpx · Pydantic.
Everything runs on local models; the total tool cost was $0.

## Earlier QA automation work

- [saucedemo-fullstack-automation-js](https://github.com/Jordy1406/saucedemo-fullstack-automation-js): Playwright + Appium + Cucumber, POM, GitHub Actions
- [automation-web-mobile-robotframework-playwright](https://github.com/Jordy1406/automation-web-mobile-robotframework-playwright): Robot Framework + Playwright for web & mobile
- [ai-quality-engineering-journey](https://github.com/Jordy1406/ai-quality-engineering-journey): learning log on testing LLM output (schema checks, pass rates)

Professional QA stack: Playwright · Selenium · Robot Framework · Postman · JMeter · K6 · Jenkins · GitHub Actions.

## Work with me

Remote AI QA / LLM evaluation roles, or fixed-scope projects: LLM red team assessment, agent pre-launch testing, LLM
eval audit, eval-as-CI setup.
[LinkedIn](https://linkedin.com/in/jordy1406)
