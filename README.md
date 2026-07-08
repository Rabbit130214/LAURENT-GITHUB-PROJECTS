**Quantitative Finance | Balance Sheet Risk | Private Credit | Applied AI**

Senior quantitative finance professional with 27 years of institutional experience
, building Python and AI-driven tools for risk management , asset and structured products valuation and Private CREDIT

## Focus areas

- **IRRBB** — interest rate risk in the banking book: gap analysis, EVE/NII
  sensitivity, behavioural modelling, regulatory stress scenarios
- **Liquidity risk** — NSFR monitoring, behavioural liquidity, funding
  stress testing, ALM integration
- **ICAAP** — capital adequacy frameworks, stress testing design, risk
  appetite calibration, regulatory reporting (Basel III/IV, CRR3)
  
- **PRIVATE CREDIT VALUATION** — IPEV methodologies, DCF and
  comparable-based fair value, PIK and covenant analytics, BDC portfolio
  analysis from FRED - SEC EDGAR public filings : PYTHON DEVELOPMENTS / MCP SERVER

  

## Current work *(private repositories — demos available on request)*

- 🔍 * 🔍 **Private credit risk intelligence engine** — multi-source architecture (FRED live, SEC EDGAR BDC 10-Q planned, ECB Data Portal planned) with:
  * **Cogniwave Credit Stress Score (CCSS)** — composite 0-100 combining HY OAS z-score, CCC-B differential z-score, yield curve slope, 3M momentum. Fully parameterizable via Pydantic (14 tunable parameters), configuration versioning, audit-ready traceability (EU AI Act compliant)
  * **REST API (FastAPI)** with 3 endpoints (`/current`, `/latest`, `/compute`), auto-generated OpenAPI 3.1 documentation, interactive Swagger UI
  * **Analytical storage** — DuckDB persisting all snapshots and calculations with the exact configuration used, enabling retroactive analysis and calibration
  * **Test coverage** — 37 pytest tests (composite + API), CI/CD ready

  **Live observation, 8 July 2026** — CCSS crossed the alert threshold at 50.18/100. CCC-B component alone contributes 57% of the score (top 3% historical z-score at +1.92σ) while HY OAS remains compressed (-1.18σ). This asymmetric divergence between the broad credit market and the stressed tail is precisely the precursor pattern to private credit default waves — quantified in real-time by the infrastructure.

## Stack technique en synthèse

| Couche | Technologies |
| Acquisition | TypeScript 5, Node.js, MCP SDK, axios, Zod
| Orchestration | Python 3.13, Pydantic v2, MCP SDK Python
| Persistance | DuckDB 
| Validation | Zod (TypeScript) + Pydantic (Python)
| Logging | JSON structuré sur stderr 
| Tests | vitest (TypeScript), pytest + pytest-asyncio (Python) |
| Qualité code | 
| Versioning | Git monorepo, GitHub privé |


## Conception et choix d'architecture

**Monorepo** — Un seul dépôt Git pour tous les sous-projets 

**MCP par source** — Chaque source de données externe (FRED, EDGAR, ECB) sera un serveur MCP indépendant en TypeScript. 

**Validation à chaque couche** — Zod côté TypeScript et Pydantic côté Python valident strictement toute donnée traversant une frontière 

**DuckDB**

**Native EU AI Act** — Architecture conçue dès l'origine pour la conformité européenne :

  
- 📊 **ALM / IRRBB analytics** — prepayment modelling , OIS compounding, 
- 🔌 **MCP servers for finance** — TypeScript Model Context Protocol servers
  connecting LLMs to market data and risk analytics

## Stack

`Python` `pandas` `NumPy` `scikit-learn` `QuantLib` `Pydantic` `SQL` `SAS`
`VBA` `TypeScript` `Node.js` — AI certification, University of Oxford

## Contact

📍 Luxembourg — open to opportunities in Switzerland , London or US
💼 https://www.linkedin.com/in/laurent-l-526287130/

