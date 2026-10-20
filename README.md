# eBay corporate finance application

**Implemented, runnable, and provisional.** The integrated application values eBay with FCFF/WACC driven by five linked annual income statements, balance sheets and cash flows. Dated assumptions and source records are editable; no network, account or third-party Python packages are required for a normal run.

Start with [the missing-data and corrections report](DATA_QUALITY_AND_MISSING_DATA.md), then [visible results](02_repository/outputs/VISIBLE_RESULTS.md) or [the standalone HTML report](02_repository/outputs/REPORT.html). The grader can inspect these without running code.

## Run from VS Code terminal

Requires Python3.10 or later. On this computer Python3.11.4 was used.

```powershell
py 02_repository/model/finance_app.py
py 02_repository/model/finance_app.py --self-test
```

If your machine uses python rather than py, replace the command name. Or run .\Run-Finance.ps1 in PowerShell. No pip installation is needed; requirements.txt documents the standard-library-only environment.

Expected output: WATCH/DEFER, provisional low/base/high about30.58/53.17/80.55 USD/share versus the September16,2026 quote109.17. Material gaps keep the action conditional. This is not an October19 current-price analysis.

```powershell
py 02_repository/model/finance_app.py --break-test
py 02_repository/model/finance_app.py --strict
```

Break-test must exit1 and refuse valuation after deliberately corrupting cash. Strict writes the provisional report then exits2 because material evidence remains incomplete. Neither is a software success exit. Normal run/self-test exit0 when checks pass.

Custom inputs/output:

```powershell
py 02_repository/model/finance_app.py --inputs 02_repository/data/finance_inputs.json --output-dir 02_repository/outputs
```

Edit scenario assumptions in JSON, save, rerun, and inspect the resulting statements and valuation. Do not overwrite historical facts without preserving source/date/basis changes. Invalid finite values, broken statements, exhausted liquidity or invalid terminal economics cause refusal.

## Where the work lives

| Item | Path |
|---|---|
| Canonical engine | 02_repository/model/finance_app.py |
| Editable facts, sources, assumptions and cases | 02_repository/data/finance_inputs.json |
| Sources and normalizations | 02_repository/data/SOURCE_LEDGER.md and BASE_YEAR_NORMALIZATION.md |
| Assumption challenges, scenario/peer policies | 02_repository/research/ |
| Report, all statements, full-precision JSON, input snapshot, validation, hashes | 02_repository/outputs/ |
| Memo draft | 05_committee_memo/MEMO_DRAFT.md |
| Validation and reproduction evidence | 07_frozen_records/ |
| Original Edition A / human checkpoint evidence | Lab03_ValuationA.md and 01_editions/ |

Five decision periods end September16,2027–2031. These are rolling12-month forecasts, not eBay fiscal-year labels. The opening is an explicitly synthetic September bridge from June public data; see the model documentation. Latest half-year operating scale is annualized and seasonality-qualified. Statements are simplified economic forecasts, not full GAAP projections.

Source-retrieval utility source_extract.py is optional and uses network. Normal valuation never downloads data. build_records.py generated explanatory records; it is not required to run the engine. It does not create human attestations.

## Reproducibility and evidence limits

Automated tests cover filing/base and accounting-basis reconciliation, statement links, closed-form known answer, WACC/g boundaries/directions, EV-equity bridge, financing independence, negative FCFF, reverse DCF, peer arithmetic and deliberate failure. Actual log is in outputs/validation.json.

Read DATA_QUALITY_AND_MISSING_DATA.md before treating this as final underwriting. Original root-level lab scripts, notes and Edition A are unchanged historical artifacts; their different dates/results are not the new model. Human AI-off/partner/recording/submission evidence remains your work. Official Brightspace checklist filenames must still be confirmed.



## Video preparation review update

Start with [VIDEO_START_HERE.md](VIDEO_START_HERE.md) and its shared fact sheet. Use numbered-folder canonical paths. Original Edition A is now [01_editions/Lab03_ValuationA.md](01_editions/Lab03_ValuationA.md). Root document copies are navigation pointers; root finance_inputs.json is NOT the engine default. Do not run historical build_records.py/finalize_patch.py as demo/finalization commands: they can overwrite current reviewed records. finance_app.py is the supported entry point.


## Supplied templates incorporated

The user supplied the exact12-row manifest, Research Evolution and Validation/AI-Use headings, transcript metadata, and memo maximum2pages (or optional8-main-slide deck). PDFs are at output/pdf/Research-Evolution.pdf, output/pdf/Validation-and-AI-Use.pdf and output/pdf/Decision-Memo.pdf. Transcript placeholders now match the supplied header. No official video time limits were included. Original Edition A PDF is not present; a text rendition is explicitly labeled rather than passed off as the original. AI closed during changed-input EXECUTION remains unconfirmed.
