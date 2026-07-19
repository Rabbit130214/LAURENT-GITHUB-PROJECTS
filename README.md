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

  

### 🔍 Private credit risk intelligence engine

Multi-source architecture: FRED live, SEC EDGAR BDC 10-Q planned, ECB Data Portal planned.

* **Cogniwave Credit Stress Score (CCSS)** — 0-100 composite over four components (HY OAS z-score, CCC-B differential z-score, yield curve slope, 3M momentum), derived from five raw FRED series
* **Fully configurable analytics** — every statistical parameter exposed through Pydantic models across three configuration layers: indicator computation (rolling windows, regime boundaries, alert percentiles), composite weighting and interpretation zones, and signal thresholds. Each computation embeds the exact configuration used, making any historical score reproducible — EU AI Act traceability by construction
* **Deterministic signal engine** — eight named rules turning a bare score into explainable observations: single-component dominance, tail/broad divergence, zone transitions, regime persistence, momentum regimes. No LLM, no heuristics — same input, same output, every threshold auditable and configurable
* **REST API** — FastAPI (`/current`, `/latest`, `/compute`), auto-generated OpenAPI 3.1, interactive Swagger UI
* **Analytical storage** — DuckDB persisting every snapshot with its configuration, enabling retroactive analysis and calibration
* **Test coverage** — 99 pytest tests across composite, indicators, signals and API layers

**Live reading, 18 July 2026** — CCSS at 51.1/100, alert zone. The CCC-B differential contributes 56% of the total score at +1.92σ (99th percentile over five years) while broad HY OAS sits at -1.07σ. The engine flags this as `SPREAD_TAIL_DIVERGENCE`: the stressed tail is repricing while the broad market stays compressed — the configuration that has historically preceded private credit default waves.


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

