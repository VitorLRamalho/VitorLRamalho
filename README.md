# Vitor Luiz Ramalho

Software developer in São Paulo, focused on **DevSecOps and application security**: security controls inside the delivery pipeline, with evidence for every decision.

Portuguese native, advanced English. Open to junior AppSec, DevSecOps or security-minded engineering roles.

## Featured: secure-tasks-api

[![DevSecOps Pipeline](https://github.com/VitorLRamalho/secure-tasks-api/actions/workflows/devsecops.yml/badge.svg)](https://github.com/VitorLRamalho/secure-tasks-api/actions/workflows/devsecops.yml)
[![OpenSSF Scorecard](https://api.scorecard.dev/projects/github.com/VitorLRamalho/secure-tasks-api/badge)](https://scorecard.dev/viewer/?uri=github.com/VitorLRamalho/secure-tasks-api)

A FastAPI service wrapped in a GitHub Actions pipeline that blocks insecure changes before they reach `main`. Built and documented in 13 days.

[![Pipeline: four parallel gates, build, image scan, SBOM, authenticated DAST, signed release](https://raw.githubusercontent.com/VitorLRamalho/secure-tasks-api/main/docs/pipeline.png)](https://github.com/VitorLRamalho/secure-tasks-api)

- Four parallel gates on every pull request: Gitleaks, Semgrep + Bandit, pip-audit + Trivy, pytest + hypothesis + atheris fuzzing.
- Build, image scan, CycloneDX SBOM and authenticated OWASP ZAP scan before `main`; keyless Cosign signature and SBOM attestation on release.
- Every action pinned to a commit SHA, hash-pinned dependencies, Dependabot with cooldown. OpenSSF Scorecard 7.5.
- [A pull request with four deliberate flaws](https://github.com/VitorLRamalho/secure-tasks-api/pull/21), blocked by every gate, then fixed one commit at a time.
- [Findings log](https://github.com/VitorLRamalho/secure-tasks-api/blob/main/docs/findings.md) with 26 recorded decisions and a [STRIDE threat model](https://github.com/VitorLRamalho/secure-tasks-api/blob/main/docs/threat-model.md). README in [English](https://github.com/VitorLRamalho/secure-tasks-api#readme) and [Portuguese](https://github.com/VitorLRamalho/secure-tasks-api/blob/main/README.pt-BR.md).

## How I work

- Evidence over checklists: a control exists when a test, a gate or a log proves it.
- Every exception has an owner, a reason and a review date.
- Supply chain is code: pin by digest and commit SHA, verify signatures, read release notes before merging a major.

## Stack

| | |
| --- | --- |
| Languages | Python (FastAPI, SQLAlchemy, Pydantic), JavaScript / Node.js, SQL |
| Security tooling | Semgrep, Bandit, Gitleaks, pip-audit, Trivy, OWASP ZAP, Syft, Cosign / Sigstore, OpenSSF Scorecard |
| Delivery | GitHub Actions, Docker (multi-stage, non-root, digest-pinned), Dependabot, branch rulesets |
| Testing | pytest, hypothesis, atheris, coverage gates |
| Methods | STRIDE threat modeling, OWASP Top 10 and API Top 10, findings logs with review dates |

## Certifications

Cisco Junior Cybersecurity Analyst Career Path (2026) · Cisco Introduction to Cybersecurity · Fortinet NSE 1, 2 and 3 · Fortinet Certified Fundamentals Cybersecurity

## Contact

[LinkedIn](https://www.linkedin.com/in/vitor-luiz-ramalho-193792247/) · vitorlramalho@gmail.com · São Paulo, Brazil
