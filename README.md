# MCB TEA and Cost Benefit

Marine Cloud Brightening: Cost, Benefit, and Planetary-Scale Assessment.

A bottom-up techno-economic assessment (TEA) of marine cloud brightening in a single Excel workbook. It uses the best available academic sources for inputs and connects them into one end-to-end assessment, then works through different delivery mechanisms: a dedicated vessel, piggybacking on a cargo ship, fixed platforms, and stationary vessels. The foundation is the numbers from Daniel Harrison's prototype on the Great Barrier Reef.

**Workbook:** `Draft MCB TEA and Cost Benefit TJ 10122026.xlsx` (draft: global benefit numbers may change once the eligible-particle cutoff is settled)

## How the workbook is organized

Start on the `Overview` tab. The workbook has two parts.

**Particle cost model (tabs 1-4): what it costs to produce and spray particles**

| Tab | What it covers |
| --- | --- |
| 1. Technology Description | The spray machine. CCN product = 30-1000 nm particles (Harrison 2025 convention). |
| 2. Cost Inputs | The blue input cells: capital, energy, crew, unit costs. |
| 3a. Outputs - Dedicated Vessel | Levelized cost per tonne of aerosol (the anchor number). |
| 3b / 3c / 3d | Cheaper siting and delivery vs a dedicated vessel: ship piggyback, fixed platform, stationary vessel. |
| 4. Scenario Comparison | Levelized cost per tonne of aerosol across 3a-3d, side by side. |

**Cooling costs and benefit (tabs 5-6): what the cooling is worth**

| Tab | What it covers |
| --- | --- |
| 5a / 5b | $/tonne into $/unit cooling, the model the benefit tabs read (5a); sensitivity tornado of that answer (5b). |
| 5c / 5c-alt / 5d | Local benefits: reef bleaching relief (5c, plus a Zhao-based alternate) and city heat deaths (5d). |
| 6a | Tonnes into global cooling via published Earth-system models. |
| 6b / 6c | Value per degree-year vs climate damage functions, for the dedicated vessel and piggyback cases. |
| References | Every paper the inputs were pulled from. |

## Legend

- Black text = formula
- Blue fill = inputs, you can change these
- Green text = pulled from another tab

## Out of scope

- Monitoring, reporting, verification (MRV): no measured forcing, no verification, no certification.
- Marine ecosystem impacts other than cooling and its effects.
- Large-scale circulation response, i.e. what cooling the Great Barrier Reef by 1C does to other parts of the climate system.

## Changes 2026-10

Review fixes. Every changed cell, with its old and new formula and value, reason and source, is listed on the new `Review changes 2026-10` tab, with a before/after table of headline outputs at the bottom. The review findings and per-input literature ranges behind them are in `review/claims_and_citations_2026-10.xlsx`.

- Local cooling: the diurnal cycle was counted twice (5a), and the reef and city fleets counted the dedicated vessel's 33% year-round spray share on top of the season (5c, 5d). Both understated MCB.
- City case (5d): cooling now comes from the 5a chain with cloud availability instead of a typed 0.8 degC, at least one whole vessel is chartered, and the mortality RR applies to all deaths on heat days.
- Global (6a): our CCN fraction is now the share activating at 0.1% supersaturation (~0.22, an estimate) to match the models' definition, model sizes use volume-mean diameters, the CESM2-Ghosh multiplier uses the equal-tonnage ratio, CESM2 efficiency is linked at 0.231.
- New explicit lines: diesel CO2 per tonne and a carbon price (tab 2, default $190/t, set 0 to exclude), shore cable for the fixed platform (3c), feasibility and SAI comparison blocks (6b, 6c), response lag factor (default 1.0) and a hot-model sensitivity (6a).
- Tornado on 3a rebuilt on the power-sized vessel. Its base now equals the headline.
- References tab: about 25 missing sources added and a few attributions fixed.

## Questions, comments, complaints

Tito Jankowski, tito.jankowski@renphil.org
