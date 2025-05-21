# ProofOfPush

> *“Show, don’t just tell — prove every résumé claim with real GitHub pushes.”*

![MIT](https://img.shields.io/badge/License-MIT-green) ![Status](https://img.shields.io/badge/status-alpha-orange)

> **Status:** 🚧 Alpha – looking for contributors.

---

## 1. Vision

A self-service, open-source verifier that **matches résumé statements with publicly verifiable GitHub activity**. We empower recruiters to skip the BS, and developers to showcase *evidence-backed* skill.

---

## 2. Problem Statement

* **Résumé Inflation** – Claims of “production-grade systems” backed by tiny forks or tutorial repos.
* **Recruiter Time Sink** – Manual code screens are slow and expensive.
* **Credible Devs Get Lost** – Genuine talent often drowns in the noise.

---

## 3. MVP Feature Set

1. **Résumé Parser** – spaCy / OpenAI to pull skills & project claims.
2. **GitHub Analyzer** – Aggregate language stats, commit volume, PR merges, issue activity.
3. **Claim Matcher** – LLM + heuristics to assign confidence scores.
4. **Credibility Dashboard** – Web UI + PDF export.
5. **Public API** – `/verify` endpoint (rate-limited) for integrators.

---

## 4. Tech Stack

| Layer    | Tech                                          |
| -------- | --------------------------------------------- |
| Backend  | Python 3.12, FastAPI, PostgreSQL (audit logs) |
| Data     | GitHub REST/GraphQL, Redis cache              |
| NLP      | spaCy + OpenAI (gpt-4o)                       |
| Frontend | Streamlit                                     |
| CI/CD    | GitHub Actions → Fly.io / AWS                 |
| Docs     | MkDocs + Material theme                       |

---


## 5. Open Questions

1. How do we fairly weight private experience vs. public activity?
2. What’s the optimal scoring formula (heuristics vs. LLM weighting)?
3. Should we gate advanced features behind a token system or sponsorship?

---

## 6. License

This project is licensed under the **MIT License** – permissive for startups & recruiters; attribution via badge appreciated.

---

