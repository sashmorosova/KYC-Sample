# EDD / Sanctions-Screening Work Samples

Two illustrative Enhanced Due Diligence (EDD) and sanctions-screening notes, written to demonstrate AML/KYC methodology on a risk-based approach consistent with the FATF 40 Recommendations. Each note is a self-contained case study built entirely from the public record of a well-known enforcement matter, with entity names disguised.

**These are work samples, not live compliance records.** All facts, amounts, and designations come from public sources; no confidential customer information is used.

## Contents

| File | Case study | Based on |
|---|---|---|
| [EDD-work-sample-Lantana.tex](EDD-work-sample-Lantana.tex) / [.pdf](EDD-work-sample-Lantana.pdf) | Lantana Trade LLP — UK LLP with a non-resident account at an Estonian branch; offshore nominee members, PEP nexus, activity inconsistent with dormant statutory filings | Danske Bank Estonia matter (Bruun & Hjejle report 2018; OCCRP; ICIJ FinCEN Files; U.S. DOJ/SEC 2022 resolution) |
| [EDD-work-sample-Meridian.tex](EDD-work-sample-Meridian.tex) / [.pdf](EDD-work-sample-Meridian.pdf) | Meridian Leaf Trading Pte. Ltd. — Singapore tobacco trader with a DPRK nexus, control-retention divestment (EUR 1 sale), and USD clearing through front companies | April 2023 OFAC/DOJ resolutions with British American Tobacco p.l.c. and BAT Marketing (Singapore) |

Both notes follow the same structure: client overview and risk classification, beneficial ownership tracing (FATF R.24/25), sanctions and watchlist screening (OFAC SDN, 50 Percent Rule, UNSCR designations), red-flag analysis, and a documented disposition (**EXIT & REPORT** in both cases).

## Methodology highlights

- Risk-based approach under FATF R.1; customer due diligence and EDD under R.10; PEP handling under R.12
- Beneficial ownership assessed as *ultimate effective control*, not registered shareholding
- Targeted financial sanctions (R.7) and proliferation-financing risk assessment per the FATF PF Guidance (June 2021)
- Each finding tied to a specific red-flag typology and a concrete recommendation

## Building the PDFs

The documents use `fontspec` (DejaVu Serif), so compile with **XeLaTeX or LuaLaTeX** — not pdflatex. Run twice so footers and references settle:

```sh
xelatex EDD-work-sample-Lantana.tex && xelatex EDD-work-sample-Lantana.tex
xelatex EDD-work-sample-Meridian.tex && xelatex EDD-work-sample-Meridian.tex
```

Required packages (all in TeX Live / MacTeX): `fontspec`, `geometry`, `xcolor`, `longtable`, `booktabs`, `enumitem`, `titlesec`, `fancyhdr`, `hyperref`, `parskip`. DejaVu Serif must be installed as a system font.

The two `.tex` files share the same template — to create a new case study, copy one and edit the header table and body sections.

## Author

Alexandra Morosova — AML/KYC / Financial Crime Analyst
