# Reference Source — the data

**80,188 checkable facts across 214 reference datasets. Every record
carries the URL it came from and the verbatim line on that page which states
it.**

Canonical home: **[referencesource.org](https://referencesource.org/)**. This
repository is a snapshot of the machine-readable exports; the site is the source
of truth and is re-verified on a schedule.

## Why the quote matters

Most reference data on the web asks you to trust it, and a plausible number is
indistinguishable from a checked one once it has been copied twice.

So beyond the value itself, every record carries:

- `source` — the page the value was taken from;
- `source_quote` — the exact sentence on that page which states it;
- `verified_fields` — the fields mechanically confirmed to appear inside that
  quote;
- `derived_fields` — the fields that are our own classification rather than the
  page's words, so you never have to guess which is which.

You can check any record here against its source without asking us anything.
That is the entire product. Where a source does not state something the row is
omitted rather than guessed, so the gaps are deliberate.

```json
{
  "state": "Massachusetts",
  "exempt_share_of_earnings": "85 per cent of the debtor's gross wages",
  "fully_exempt_threshold": "50 times the greater of the federal or the Massachusetts hourly minimum wage",
  "statute_section": "Section 28: Wages and pensions; exemptions; exceptions",
  "url": "https://referencesource.org/wage-garnishment-exemption-thresholds-by-state/massachusetts/",
  "source": "https://malegislature.gov/Laws/GeneralLaws/PartIII/TitleIV/Chapter246/Section28",
  "source_quote": "attached for a debt or claim, an amount not exceeding the greater of 85 per cent of the debtor's gross wages or 50 times the greater of the federal or the Massachusetts hourly minimum wage for each week or portion thereof out of the wages then due to the defendant for labor performed or se",
  "verified_fields": ["exempt_share_of_earnings", "fully_exempt_threshold", "statute_section"],
  "derived_fields": ["state"]
}
```

## Layout

```
catalog.json        every dataset: name, description, record count, last
                    verified date, canonical URL
<slug>/data.json    one dataset — metadata, licence position, sources, records
<slug>/README.md    what it covers, when it was last verified, canonical link
```

## Freshness, and what "verified" does not mean

Reference data decays, and the re-checking is the part that matters rather than
the assembling. Every dataset carries `last_verified` and `stale_after`.
Verification means the value was mechanically confirmed to appear inside the
quoted line, and the quote to appear on the page — **not** that a human has
adjudicated the underlying question. What that does and does not cover:
[referencesource.org/method/](https://referencesource.org/method/)

For current data read the site. Each dataset publishes an Atom feed of what
changed, so you can poll instead of re-fetching. There is an MCP server —
[`referencesource-mcp`](https://www.npmjs.com/package/referencesource-mcp) — and
a machine entry point at
[referencesource.org/llms.txt](https://referencesource.org/llms.txt).

## Coverage is uneven, on purpose

Datasets are built until their sources are exhausted, which takes more than one
pass, and a dataset covering part of its territory is not claiming to be
complete. Where a jurisdiction is missing it is usually because its source could
not be read from an official host; the dataset's `sources` list normally names
what was left out and why.

## Licence and attribution

The facts and this compilation are free to use, including commercially;
attribution to referencesource.org is requested. Individual facts are not
copyrightable (*Feist*, 499 U.S. 340 (1991)); the selection and verification are
ours and are licensed on those terms, matching the machine-readable position at
[license.xml](https://referencesource.org/license.xml).

`source_quote` fields are short verbatim excerpts from the publishers named in
`source`, reproduced so a reader can check the value. We claim no rights over
them, they are attributed and linked in every record, and they exist to send you
to the original rather than replace it. Where a source's own terms govern reuse
those terms govern — several datasets record a `licence` position saying exactly
that. We do not mirror whole compilations from publishers whose product *is* the
compilation: we record the fact and link the document.

## Corrections

If a record is wrong that is worth more to us than one that is right. Open an
issue with the dataset, the record and the source URL — anything found wrong gets
fixed or pulled rather than left up.

## Datasets


| Dataset | Records | Last verified | Canonical |
|---|---:|---|---|
| [Withdrawn and superseded ISO standards](iso-standard-supersessions/) | 24,542 | 2026-08-05 | [referencesource.org/iso-standard-supersessions/](https://referencesource.org/iso-standard-supersessions/) |
| [FIPS 140 validated cryptographic modules: active, historical or revoked](fips-140-module-validation-status/) | 5,492 | 2026-08-26 | [referencesource.org/fips-140-module-validation-status/](https://referencesource.org/fips-140-module-validation-status/) |
| [Which OSHA-recognized labs (NRTLs) can certify to a given test standard](nrtl-recognized-test-standards/) | 4,329 | 2026-08-10 | [referencesource.org/nrtl-recognized-test-standards/](https://referencesource.org/nrtl-recognized-test-standards/) |
| [Domain registrar accreditation status and ICANN enforcement history, by IANA ID](icann-registrar-accreditation-status/) | 4,324 | 2026-08-06 | [referencesource.org/icann-registrar-accreditation-status/](https://referencesource.org/icann-registrar-accreditation-status/) |
| [Which OSHA NRTL is recognized for which test standard: all 21 labs' scopes of recognition, cross-referenced](nrtl-recognition-scopes/) | 3,321 | 2026-08-10 | [referencesource.org/nrtl-recognition-scopes/](https://referencesource.org/nrtl-recognition-scopes/) |
| [2026 conforming loan limits by county: one- to four-unit properties](conforming-loan-limits/) | 3,235 | 2026-08-10 | [referencesource.org/conforming-loan-limits/](https://referencesource.org/conforming-loan-limits/) |
| [IECC/Building America climate zone by U.S. county, 2021 code cycle](iecc-climate-zone-by-county/) | 3,134 | 2026-08-19 | [referencesource.org/iecc-climate-zone-by-county/](https://referencesource.org/iecc-climate-zone-by-county/) |
| [Mailing and air-carriage restrictions by item category](shipping-restrictions-by-class/) | 2,852 | 2026-08-10 | [referencesource.org/shipping-restrictions-by-class/](https://referencesource.org/shipping-restrictions-by-class/) |
| [Chemical resistance ratings for common elastomers](chemical-elastomer-material-compatibility/) | 2,086 | 2026-08-12 | [referencesource.org/chemical-elastomer-material-compatibility/](https://referencesource.org/chemical-elastomer-material-compatibility/) |
| [Nursing homes under CMS Special Focus Facility oversight: current SFFs, candidates, graduates and terminations, by CMS certification number](nursing-home-special-focus-facilities/) | 1,927 | 2026-08-11 | [referencesource.org/nursing-home-special-focus-facilities/](https://referencesource.org/nursing-home-special-focus-facilities/) |
| [Federal Reserve enforcement actions against banks and holding companies: action type, effective date and whether it has been terminated](bank-enforcement-actions/) | 1,558 | 2026-08-11 | [referencesource.org/bank-enforcement-actions/](https://referencesource.org/bank-enforcement-actions/) |
| [Vehicle inspection defect categories: MOT major, minor and dangerous verdicts](vehicle-inspection-defect-categories/) | 1,422 | 2026-08-06 | [referencesource.org/vehicle-inspection-defect-categories/](https://referencesource.org/vehicle-inspection-defect-categories/) |
| [US federal chemical regulatory reporting thresholds by program (CERCLA, EPCRA, CAA)](chemical-regulatory-reporting-thresholds/) | 1,336 | 2026-08-05 | [referencesource.org/chemical-regulatory-reporting-thresholds/](https://referencesource.org/chemical-regulatory-reporting-thresholds/) |
| [US EPA pesticide residue tolerance limits by active ingredient and crop commodity](pesticide-residue-tolerance-limits/) | 1,324 | 2026-08-17 | [referencesource.org/pesticide-residue-tolerance-limits/](https://referencesource.org/pesticide-residue-tolerance-limits/) |
| [Hospital price-transparency machine-readable file index (cms-hpt.txt)](hospital-price-transparency-mrf-index/) | 950 | 2026-08-18 | [referencesource.org/hospital-price-transparency-mrf-index/](https://referencesource.org/hospital-price-transparency-mrf-index/) |
| [US workplace chemical exposure limits: federal OSHA vs Cal/OSHA, side by side](workplace-exposure-limits/) | 886 | 2026-08-05 | [referencesource.org/workplace-exposure-limits/](https://referencesource.org/workplace-exposure-limits/) |
| [Consumer router firmware support — end-of-life status and dates by vendor and model](router-firmware-support-status/) | 880 | 2026-08-11 | [referencesource.org/router-firmware-support-status/](https://referencesource.org/router-firmware-support-status/) |
| [Stihl chainsaw chain and bar specifications by model](stihl-chainsaw-chain-and-bar-specs/) | 809 | 2026-08-05 | [referencesource.org/stihl-chainsaw-chain-and-bar-specs/](https://referencesource.org/stihl-chainsaw-chain-and-bar-specs/) |
| [ESAB recommended filler metals and suggested preheat group, by ASTM steel grade](esab-filler-metal-recommendations-by-astm-steel-grade/) | 794 | 2026-08-19 | [referencesource.org/esab-filler-metal-recommendations-by-astm-steel-grade/](https://referencesource.org/esab-filler-metal-recommendations-by-astm-steel-grade/) |
| [Hazmat load segregation — which hazard classes may travel together, highway vs vessel](hazmat-segregation-matrix/) | 788 | 2026-08-10 | [referencesource.org/hazmat-segregation-matrix/](https://referencesource.org/hazmat-segregation-matrix/) |
| [State Insurance Department Complaint Index by Company](state-insurance-complaint-index-by-company/) | 622 | 2026-08-26 | [referencesource.org/state-insurance-complaint-index-by-company/](https://referencesource.org/state-insurance-complaint-index-by-company/) |
| [Federal civil penalty maximums — current inflation-adjusted amounts across agencies](federal-civil-penalty-maximums/) | 574 | 2026-08-10 | [referencesource.org/federal-civil-penalty-maximums/](https://referencesource.org/federal-civil-penalty-maximums/) |
| [Planned US generating-unit retirements, as EIA published them in one named month's Electric Power Monthly](power-plant-retirement-schedule/) | 484 | 2026-08-18 | [referencesource.org/power-plant-retirement-schedule/](https://referencesource.org/power-plant-retirement-schedule/) |
| [Food additive regulatory approval status — US FDA vs EU](food-additive-approval-status-us-vs-eu/) | 479 | 2026-08-18 | [referencesource.org/food-additive-approval-status-us-vs-eu/](https://referencesource.org/food-additive-approval-status-us-vs-eu/) |
| [Current EPA nonattainment county designations by pollutant](nonattainment-county-designations-by-pollutant/) | 463 | 2026-08-24 | [referencesource.org/nonattainment-county-designations-by-pollutant/](https://referencesource.org/nonattainment-county-designations-by-pollutant/) |
| [FDA import alert red lists: firms subject to detention without physical examination](fda-import-alert-red-list/) | 424 | 2026-08-06 | [referencesource.org/fda-import-alert-red-list/](https://referencesource.org/fda-import-alert-red-list/) |
| [Interstate Professional Licensure Compact Participation by State](interstate-licensure-compact-participation/) | 406 | 2026-08-17 | [referencesource.org/interstate-licensure-compact-participation/](https://referencesource.org/interstate-licensure-compact-participation/) |
| [AI model deprecation and retirement dates by provider](ai-model-deprecation-and-retirement/) | 347 | 2026-08-12 | [referencesource.org/ai-model-deprecation-and-retirement/](https://referencesource.org/ai-model-deprecation-and-retirement/) |
| [Industrial VFD fault and alarm codes by brand](industrial-vfd-fault-alarm-codes-by-brand/) | 340 | 2026-08-26 | [referencesource.org/industrial-vfd-fault-alarm-codes-by-brand/](https://referencesource.org/industrial-vfd-fault-alarm-codes-by-brand/) |
| [TOEFL iBT score equivalence: IELTS bands, CEFR levels and the 2026 1–6 scale, as published by ETS](english-test-score-equivalence/) | 336 | 2026-08-11 | [referencesource.org/english-test-score-equivalence/](https://referencesource.org/english-test-score-equivalence/) |
| [US state notifiable disease reporting timeframes by condition](notifiable-disease-reporting-timeframes/) | 334 | 2026-08-16 | [referencesource.org/notifiable-disease-reporting-timeframes/](https://referencesource.org/notifiable-disease-reporting-timeframes/) |
| [Power tool battery platform and accessory interface compatibility](power-tool-battery-compatibility/) | 273 | 2026-08-11 | [referencesource.org/power-tool-battery-compatibility/](https://referencesource.org/power-tool-battery-compatibility/) |
| [Software interface version compatibility](software-interface-version-compatibility/) | 248 | 2026-08-11 | [referencesource.org/software-interface-version-compatibility/](https://referencesource.org/software-interface-version-compatibility/) |
| [Civil statute of limitations by state and type of claim](state-civil-statute-of-limitations/) | 238 | 2026-08-25 | [referencesource.org/state-civil-statute-of-limitations/](https://referencesource.org/state-civil-statute-of-limitations/) |
| [Federal rules taking effect: every published US final rule whose effective date is still in the future](federal-rules-taking-effect/) | 234 | 2026-08-10 | [referencesource.org/federal-rules-taking-effect/](https://referencesource.org/federal-rules-taking-effect/) |
| [File format magic numbers](file-format-signatures/) | 229 | 2026-08-03 | [referencesource.org/file-format-signatures/](https://referencesource.org/file-format-signatures/) |
| [OSHA PSM vs EPA RMP: chemical threshold quantities side by side](psm-rmp-chemical-threshold-crossref/) | 225 | 2026-08-15 | [referencesource.org/psm-rmp-chemical-threshold-crossref/](https://referencesource.org/psm-rmp-chemical-threshold-crossref/) |
| [VOC content limits for architectural coatings by jurisdiction](voc-limits-architectural-coatings/) | 222 | 2026-08-06 | [referencesource.org/voc-limits-architectural-coatings/](https://referencesource.org/voc-limits-architectural-coatings/) |
| [AP exam score to college credit, compared across universities](ap-exam-credit-by-university/) | 221 | 2026-08-05 | [referencesource.org/ap-exam-credit-by-university/](https://referencesource.org/ap-exam-credit-by-university/) |
| [Pilot licence minimum hours, age and prerequisites by civil aviation authority](pilot-licence-minimum-requirements-by-authority/) | 203 | 2026-08-10 | [referencesource.org/pilot-licence-minimum-requirements-by-authority/](https://referencesource.org/pilot-licence-minimum-requirements-by-authority/) |
| [Camera mount flange focal distance and adapter feasibility](camera-lens-body-adapter-compatibility/) | 201 | 2026-08-13 | [referencesource.org/camera-lens-body-adapter-compatibility/](https://referencesource.org/camera-lens-body-adapter-compatibility/) |
| [Certification marks and hazardous-area classifications: cross-market equivalences](certification-standards-equivalence/) | 200 | 2026-08-11 | [referencesource.org/certification-standards-equivalence/](https://referencesource.org/certification-standards-equivalence/) |
| [Carbide insert grade cross-reference by ISO application group and manufacturer](carbide-insert-grade-cross-reference/) | 184 | 2026-08-11 | [referencesource.org/carbide-insert-grade-cross-reference/](https://referencesource.org/carbide-insert-grade-cross-reference/) |
| [Drinking water contaminant limits by regulator](drinking-water-contaminant-limits/) | 182 | 2026-08-06 | [referencesource.org/drinking-water-contaminant-limits/](https://referencesource.org/drinking-water-contaminant-limits/) |
| [Appliance fault and error codes](appliance-fault-error-codes/) | 170 | 2026-08-04 | [referencesource.org/appliance-fault-error-codes/](https://referencesource.org/appliance-fault-error-codes/) |
| [Fastener standard equivalences: DIN to ISO / EN crossover](fastener-thread-standard-equivalence/) | 164 | 2026-08-12 | [referencesource.org/fastener-thread-standard-equivalence/](https://referencesource.org/fastener-thread-standard-equivalence/) |
| [FAA flight training hour minimums: Part 61 vs Part 141, by certificate and rating](flight-training-hour-minimums-61-vs-141/) | 164 | 2026-08-19 | [referencesource.org/flight-training-hour-minimums-61-vs-141/](https://referencesource.org/flight-training-hour-minimums-61-vs-141/) |
| [DIN / ISO / BS fastener equivalents and the sizes where they are not interchangeable](fastener-standard-interchangeability-exceptions/) | 162 | 2026-08-05 | [referencesource.org/fastener-standard-interchangeability-exceptions/](https://referencesource.org/fastener-standard-interchangeability-exceptions/) |
| [Power tool battery and accessory compatibility](power-tool-battery-accessory-compatibility/) | 149 | 2026-08-11 | [referencesource.org/power-tool-battery-accessory-compatibility/](https://referencesource.org/power-tool-battery-accessory-compatibility/) |
| [Superseded and deprecated identifier mappings](superseded-standards-mappings/) | 141 | 2026-08-04 | [referencesource.org/superseded-standards-mappings/](https://referencesource.org/superseded-standards-mappings/) |
| [CLEP exam credit policies by university](clep-credit-by-university/) | 130 | 2026-08-18 | [referencesource.org/clep-credit-by-university/](https://referencesource.org/clep-credit-by-university/) |
| [EPA national recommended water quality criteria for human health: pollutant concentration thresholds](epa-water-quality-criteria-human-health/) | 127 | 2026-08-19 | [referencesource.org/epa-water-quality-criteria-human-health/](https://referencesource.org/epa-water-quality-criteria-human-health/) |
| [Texas electrician licensing: practice questions with the answer quoted from TDLR](texas-electrician-licensing-practice-questions/) | 127 | 2026-08-25 | [referencesource.org/texas-electrician-licensing-practice-questions/](https://referencesource.org/texas-electrician-licensing-practice-questions/) |
| [EPA NESHAP Source Category Applicability Crosswalk](neshap-source-category-crosswalk/) | 125 | 2026-08-15 | [referencesource.org/neshap-source-category-crosswalk/](https://referencesource.org/neshap-source-category-crosswalk/) |
| [Blood donor deferral criteria compared across national blood services](blood-donor-deferral-criteria/) | 111 | 2026-08-13 | [referencesource.org/blood-donor-deferral-criteria/](https://referencesource.org/blood-donor-deferral-criteria/) |
| [Packaging specification equivalence: neck finishes, corrugated grades and pallet standards](packaging-material-specification-equivalence/) | 111 | 2026-08-12 | [referencesource.org/packaging-material-specification-equivalence/](https://referencesource.org/packaging-material-specification-equivalence/) |
| [HVAC refrigerant replacements: retrofit compatibility, safety class, GWP and lubricant](hvac-component-refrigerant-compatibility/) | 109 | 2026-08-11 | [referencesource.org/hvac-component-refrigerant-compatibility/](https://referencesource.org/hvac-component-refrigerant-compatibility/) |
| [Solar inverter–battery compatibility](solar-inverter-panel-battery-compatibility/) | 101 | 2026-08-12 | [referencesource.org/solar-inverter-panel-battery-compatibility/](https://referencesource.org/solar-inverter-panel-battery-compatibility/) |
| [US state PFAS product restriction effective dates by category](state-pfas-product-restrictions/) | 101 | 2026-08-14 | [referencesource.org/state-pfas-product-restrictions/](https://referencesource.org/state-pfas-product-restrictions/) |
| [PFAS drinking water concentration limits by US state — MCLs, notification levels, action levels, and health advisories for PFOA, PFOS, and other per- and polyfluoroalkyl substances](pfas-drinking-water-limits-by-state/) | 100 | 2026-08-14 | [referencesource.org/pfas-drinking-water-limits-by-state/](https://referencesource.org/pfas-drinking-water-limits-by-state/) |
| [Plumbing fitting and pipe thread standards](plumbing-fitting-thread-standards/) | 97 | 2026-08-12 | [referencesource.org/plumbing-fitting-thread-standards/](https://referencesource.org/plumbing-fitting-thread-standards/) |
| [FMCSA commercial driver disqualification offenses and periods](cdl-disqualification-offenses-and-periods/) | 96 | 2026-08-19 | [referencesource.org/cdl-disqualification-offenses-and-periods/](https://referencesource.org/cdl-disqualification-offenses-and-periods/) |
| [Deprecated npm packages and their maintainer-named replacement](npm-deprecated-package-recommended-replacement/) | 96 | 2026-08-25 | [referencesource.org/npm-deprecated-package-recommended-replacement/](https://referencesource.org/npm-deprecated-package-recommended-replacement/) |
| [Firewall and network security appliance hardware end-of-life dates by brand](firewall-hardware-end-of-life-dates-by-brand/) | 93 | 2026-08-26 | [referencesource.org/firewall-hardware-end-of-life-dates-by-brand/](https://referencesource.org/firewall-hardware-end-of-life-dates-by-brand/) |
| [FDA nutrient content claim qualification criteria](fda-nutrient-content-claim-criteria/) | 90 | 2026-08-17 | [referencesource.org/fda-nutrient-content-claim-criteria/](https://referencesource.org/fda-nutrient-content-claim-criteria/) |
| [Assisted living facility minimum staffing requirements by US state — how many staff must be on duty, and what that guarantees](assisted-living-facility-staffing-ratios-by-state/) | 85 | 2026-08-19 | [referencesource.org/assisted-living-facility-staffing-ratios-by-state/](https://referencesource.org/assisted-living-facility-staffing-ratios-by-state/) |
| [Bike drivetrain and groupset compatibility](bike-drivetrain-groupset-compatibility/) | 85 | 2026-08-11 | [referencesource.org/bike-drivetrain-groupset-compatibility/](https://referencesource.org/bike-drivetrain-groupset-compatibility/) |
| [OSHA injury and illness recordkeeping exemptions by industry (NAICS)](osha-recordkeeping-exemptions/) | 82 | 2026-08-19 | [referencesource.org/osha-recordkeeping-exemptions/](https://referencesource.org/osha-recordkeeping-exemptions/) |
| [US state unclaimed property dormancy periods by property type](state-unclaimed-property-dormancy-periods/) | 81 | 2026-08-15 | [referencesource.org/state-unclaimed-property-dormancy-periods/](https://referencesource.org/state-unclaimed-property-dormancy-periods/) |
| [Galvanic series and surface energy of engineering materials](process-compatibility-coatings-adhesives-treatments/) | 80 | 2026-08-04 | [referencesource.org/process-compatibility-coatings-adhesives-treatments/](https://referencesource.org/process-compatibility-coatings-adhesives-treatments/) |
| [US AIM Act sector-specific refrigerant GWP limits and compliance dates (40 CFR 84.54)](aim-act-refrigerant-gwp-sector-limits/) | 71 | 2026-08-06 | [referencesource.org/aim-act-refrigerant-gwp-sector-limits/](https://referencesource.org/aim-act-refrigerant-gwp-sector-limits/) |
| [Accuracy classes and maximum permissible errors for trade measuring instruments (EU MID)](legal-metrology-accuracy-classes/) | 70 | 2026-08-05 | [referencesource.org/legal-metrology-accuracy-classes/](https://referencesource.org/legal-metrology-accuracy-classes/) |
| [Software end-of-support dates](software-end-of-support/) | 68 | 2026-08-03 | [referencesource.org/software-end-of-support/](https://referencesource.org/software-end-of-support/) |
| [How often hazmat cylinders, cargo tanks, IBCs and portable tanks must be retested](hazmat-container-retest-intervals/) | 67 | 2026-08-10 | [referencesource.org/hazmat-container-retest-intervals/](https://referencesource.org/hazmat-container-retest-intervals/) |
| [State employment law headcount triggers that deviate from federal thresholds](state-employment-law-headcount-triggers/) | 66 | 2026-08-14 | [referencesource.org/state-employment-law-headcount-triggers/](https://referencesource.org/state-employment-law-headcount-triggers/) |
| [North American vs IEC/ATEX explosion protection designations](ex-classification-system-crosswalk/) | 65 | 2026-08-06 | [referencesource.org/ex-classification-system-crosswalk/](https://referencesource.org/ex-classification-system-crosswalk/) |
| [Gas group, temperature class and autoignition temperature by substance](hazardous-area-substance-classification/) | 60 | 2026-08-06 | [referencesource.org/hazardous-area-substance-classification/](https://referencesource.org/hazardous-area-substance-classification/) |
| [US minimum wage rates by state, city, and worker type](minimum-wage-rates-by-jurisdiction/) | 60 | 2026-08-12 | [referencesource.org/minimum-wage-rates-by-jurisdiction/](https://referencesource.org/minimum-wage-rates-by-jurisdiction/) |
| [Deadlines to notify or sue a government body, by state](government-tort-claim-notice-deadlines-by-state/) | 59 | 2026-08-26 | [referencesource.org/government-tort-claim-notice-deadlines-by-state/](https://referencesource.org/government-tort-claim-notice-deadlines-by-state/) |
| [US boiler and pressure vessel inspection requirements by state](boiler-inspection-requirements-by-state/) | 55 | 2026-08-05 | [referencesource.org/boiler-inspection-requirements-by-state/](https://referencesource.org/boiler-inspection-requirements-by-state/) |
| [Outboard motor service specifications by brand and model](outboard-motor-service-specs/) | 53 | 2026-08-05 | [referencesource.org/outboard-motor-service-specs/](https://referencesource.org/outboard-motor-service-specs/) |
| [PDMP Mandatory Prescriber Check Requirements by State](pdmp-mandatory-check-requirements/) | 53 | 2026-08-17 | [referencesource.org/pdmp-mandatory-check-requirements/](https://referencesource.org/pdmp-mandatory-check-requirements/) |
| [CPA continuing professional education (CPE) requirements by US jurisdiction](professional-licensing-continuing-education-by-jurisdiction/) | 53 | 2026-08-12 | [referencesource.org/professional-licensing-continuing-education-by-jurisdiction/](https://referencesource.org/professional-licensing-continuing-education-by-jurisdiction/) |
| [State public works payment and performance bond thresholds (Little Miller Acts)](state-public-works-bond-thresholds/) | 53 | 2026-08-17 | [referencesource.org/state-public-works-bond-thresholds/](https://referencesource.org/state-public-works-bond-thresholds/) |
| [Minimum auto liability insurance limits by state](auto-insurance-minimums/) | 51 | 2026-08-10 | [referencesource.org/auto-insurance-minimums/](https://referencesource.org/auto-insurance-minimums/) |
| [US graduated driver licensing requirements by state](graduated-driver-licensing/) | 51 | 2026-08-05 | [referencesource.org/graduated-driver-licensing/](https://referencesource.org/graduated-driver-licensing/) |
| [Mechanics lien filing deadlines, preliminary notice requirements, and enforcement windows by US state and party role](mechanics-lien-deadlines-by-state/) | 51 | 2026-08-14 | [referencesource.org/mechanics-lien-deadlines-by-state/](https://referencesource.org/mechanics-lien-deadlines-by-state/) |
| [Nursing home minimum staffing requirements by US state — hours per resident day and RN coverage mandates after the 2026 federal repeal](nursing-home-minimum-staffing-by-state/) | 51 | 2026-08-15 | [referencesource.org/nursing-home-minimum-staffing-by-state/](https://referencesource.org/nursing-home-minimum-staffing-by-state/) |
| [Certificate of need programs by US state](state-certificate-of-need-programs/) | 51 | 2026-08-19 | [referencesource.org/state-certificate-of-need-programs/](https://referencesource.org/state-certificate-of-need-programs/) |
| [State health insurance marketplace assistance by state: who runs it, where subsidies start and stop, and what the state adds](state-marketplace-assistance-programs/) | 51 | 2026-08-19 | [referencesource.org/state-marketplace-assistance-programs/](https://referencesource.org/state-marketplace-assistance-programs/) |
| [State conformity to federal Section 179 and bonus depreciation rules](state-section-179-bonus-depreciation-conformity/) | 51 | 2026-08-15 | [referencesource.org/state-section-179-bonus-depreciation-conformity/](https://referencesource.org/state-section-179-bonus-depreciation-conformity/) |
| [Food color additive cross-reference: US FD&C designation vs EU E-number, with regulatory status comparison](food-color-additive-status-us-vs-eu/) | 50 | 2026-08-10 | [referencesource.org/food-color-additive-status-us-vs-eu/](https://referencesource.org/food-color-additive-status-us-vs-eu/) |
| [ACA marketplace subsidy income limits by coverage year, household size and state group](marketplace-subsidy-income-thresholds/) | 48 | 2026-08-13 | [referencesource.org/marketplace-subsidy-income-thresholds/](https://referencesource.org/marketplace-subsidy-income-thresholds/) |
| [Home Energy Rebates — is my state's programme open, and what does it still pay for?](home-energy-rebate-program-status-by-state/) | 47 | 2026-08-25 | [referencesource.org/home-energy-rebate-program-status-by-state/](https://referencesource.org/home-energy-rebate-program-status-by-state/) |
| [GC column stationary phase cross-reference by manufacturer](lab-instrument-consumables-equivalence/) | 47 | 2026-08-15 | [referencesource.org/lab-instrument-consumables-equivalence/](https://referencesource.org/lab-instrument-consumables-equivalence/) |
| [SNAP gross income and asset limits by US state (BBCE)](snap-gross-income-limits-by-state/) | 47 | 2026-08-19 | [referencesource.org/snap-gross-income-limits-by-state/](https://referencesource.org/snap-gross-income-limits-by-state/) |
| [Vehicle trade-in sales tax credit rules by state -- full price taxed, or only the difference](vehicle-trade-in-sales-tax-credit-by-state/) | 47 | 2026-08-20 | [referencesource.org/vehicle-trade-in-sales-tax-credit-by-state/](https://referencesource.org/vehicle-trade-in-sales-tax-credit-by-state/) |
| [How long before a car left on your property or towed from it can legally be sold — by US state](abandoned-vehicle-private-property-timelines-by-state/) | 45 | 2026-08-19 | [referencesource.org/abandoned-vehicle-private-property-timelines-by-state/](https://referencesource.org/abandoned-vehicle-private-property-timelines-by-state/) |
| [TLS certificate and CA requirement effective dates (CA/Browser Forum, Chrome, Mozilla)](tls-certificate-requirement-effective-dates/) | 45 | 2026-08-05 | [referencesource.org/tls-certificate-requirement-effective-dates/](https://referencesource.org/tls-certificate-requirement-effective-dates/) |
| [Construction prompt payment act deadlines by US state — owner-to-contractor and contractor-to-subcontractor payment windows, retention release deadlines, and late-payment interest rates](construction-prompt-payment-deadlines-by-state/) | 43 | 2026-08-15 | [referencesource.org/construction-prompt-payment-deadlines-by-state/](https://referencesource.org/construction-prompt-payment-deadlines-by-state/) |
| [LIHEAP income eligibility limits by state and household size](liheap-income-eligibility-by-state/) | 43 | 2026-08-25 | [referencesource.org/liheap-income-eligibility-by-state/](https://referencesource.org/liheap-income-eligibility-by-state/) |
| [State construction apprentice-to-journeyman ratio requirements by trade](state-apprenticeship-ratios-by-trade/) | 43 | 2026-08-15 | [referencesource.org/state-apprenticeship-ratios-by-trade/](https://referencesource.org/state-apprenticeship-ratios-by-trade/) |
| [HFC refrigerant GWP regulations by US state](hfc-refrigerant-regulations-by-state/) | 42 | 2026-08-05 | [referencesource.org/hfc-refrigerant-regulations-by-state/](https://referencesource.org/hfc-refrigerant-regulations-by-state/) |
| [How long an insurer has to acknowledge, decide and pay a claim, by state: statutory and regulatory claim-handling deadlines](insurance-claim-handling-deadlines/) | 42 | 2026-08-11 | [referencesource.org/insurance-claim-handling-deadlines/](https://referencesource.org/insurance-claim-handling-deadlines/) |
| [OSHA fall protection trigger height by standard](osha-fall-protection-trigger-height-by-standard/) | 42 | 2026-08-25 | [referencesource.org/osha-fall-protection-trigger-height-by-standard/](https://referencesource.org/osha-fall-protection-trigger-height-by-standard/) |
| [What a food must legally contain to use its name: FDA standards of identity, in one table](food-standards-of-identity/) | 41 | 2026-08-11 | [referencesource.org/food-standards-of-identity/](https://referencesource.org/food-standards-of-identity/) |
| [State Residential Radon Disclosure, Testing, and Certification Requirements](state-radon-disclosure-requirements/) | 41 | 2026-08-15 | [referencesource.org/state-radon-disclosure-requirements/](https://referencesource.org/state-radon-disclosure-requirements/) |
| [Respirator assigned protection factors — federal OSHA and Cal/OSHA, with maximum use concentrations](respirator-assigned-protection-factors/) | 40 | 2026-08-10 | [referencesource.org/respirator-assigned-protection-factors/](https://referencesource.org/respirator-assigned-protection-factors/) |
| [What a newspaper may legally charge to publish a legal notice — by US state](legal-notice-publication-rates-by-state/) | 37 | 2026-08-19 | [referencesource.org/legal-notice-publication-rates-by-state/](https://referencesource.org/legal-notice-publication-rates-by-state/) |
| [What must pass before the next step: mandated step order in regulated processes](prerequisite-sequencing-regulated-processes/) | 37 | 2026-08-11 | [referencesource.org/prerequisite-sequencing-regulated-processes/](https://referencesource.org/prerequisite-sequencing-regulated-processes/) |
| [Fire extinguisher inspection, maintenance and hydrostatic test intervals by agent type](fire-extinguisher-inspection-testing-intervals-by-type/) | 34 | 2026-08-19 | [referencesource.org/fire-extinguisher-inspection-testing-intervals-by-type/](https://referencesource.org/fire-extinguisher-inspection-testing-intervals-by-type/) |
| [Pseudoephedrine purchase limits: federal gram limits and stricter state rules](pseudoephedrine-purchase-limits-by-state/) | 34 | 2026-08-19 | [referencesource.org/pseudoephedrine-purchase-limits-by-state/](https://referencesource.org/pseudoephedrine-purchase-limits-by-state/) |
| [US federal employment law thresholds by employee count](regulatory-threshold-triggers/) | 32 | 2026-08-04 | [referencesource.org/regulatory-threshold-triggers/](https://referencesource.org/regulatory-threshold-triggers/) |
| [State insurer-of-last-resort programs — FAIR Plan / Citizens eligibility and coverage limits](state-insurer-of-last-resort-coverage-limits/) | 32 | 2026-08-19 | [referencesource.org/state-insurer-of-last-resort-coverage-limits/](https://referencesource.org/state-insurer-of-last-resort-coverage-limits/) |
| [OSHA training requirements by standard: topic, frequency, and CFR citation](osha-training-requirements-by-standard/) | 31 | 2026-08-05 | [referencesource.org/osha-training-requirements-by-standard/](https://referencesource.org/osha-training-requirements-by-standard/) |
| [Consumer contract cooling-off and rescission periods by US state and transaction type](state-consumer-cooling-off-periods/) | 31 | 2026-08-18 | [referencesource.org/state-consumer-cooling-off-periods/](https://referencesource.org/state-consumer-cooling-off-periods/) |
| [Construction retainage limits by US state — maximum withholding percentages, release deadlines, escrow requirements, and public vs private distinctions with statutory citations](construction-retainage-limits-by-state/) | 30 | 2026-08-17 | [referencesource.org/construction-retainage-limits-by-state/](https://referencesource.org/construction-retainage-limits-by-state/) |
| [How far off a US fuel pump, LPG meter or EV charger is allowed to be (NIST Handbook 44)](motor-fuel-dispenser-measurement-tolerances-nist/) | 30 | 2026-08-20 | [referencesource.org/motor-fuel-dispenser-measurement-tolerances-nist/](https://referencesource.org/motor-fuel-dispenser-measurement-tolerances-nist/) |
| [US state hazardous waste generator annual fees by category](hazardous-waste-generator-fees-by-state/) | 29 | 2026-08-16 | [referencesource.org/hazardous-waste-generator-fees-by-state/](https://referencesource.org/hazardous-waste-generator-fees-by-state/) |
| [Discontinued electronic component replacement mapping](discontinued-part-replacement-mapping/) | 28 | 2026-08-03 | [referencesource.org/discontinued-part-replacement-mapping/](https://referencesource.org/discontinued-part-replacement-mapping/) |
| [Vehicle emissions testing: which counties require it, in which states](vehicle-emissions-testing-by-state/) | 28 | 2026-08-25 | [referencesource.org/vehicle-emissions-testing-by-state/](https://referencesource.org/vehicle-emissions-testing-by-state/) |
| [State insurance mandates for fertility treatment and IVF coverage](state-fertility-insurance-mandates/) | 26 | 2026-08-17 | [referencesource.org/state-fertility-insurance-mandates/](https://referencesource.org/state-fertility-insurance-mandates/) |
| [US import duty and tariff rates by HTS chapter](import-duty-and-tariffs/) | 25 | 2026-08-15 | [referencesource.org/import-duty-and-tariffs/](https://referencesource.org/import-duty-and-tariffs/) |
| [Small Claims Court Dollar Limits by State](small-claims-court-dollar-limits-by-state/) | 25 | 2026-08-26 | [referencesource.org/small-claims-court-dollar-limits-by-state/](https://referencesource.org/small-claims-court-dollar-limits-by-state/) |
| [SSI state supplement amounts by state and living arrangement](ssi-state-supplement-amounts-by-state/) | 25 | 2026-08-19 | [referencesource.org/ssi-state-supplement-amounts-by-state/](https://referencesource.org/ssi-state-supplement-amounts-by-state/) |
| [State OSHA plan civil penalty maximums by violation type compared with federal](state-osha-plan-penalty-maximums/) | 25 | 2026-08-15 | [referencesource.org/state-osha-plan-penalty-maximums/](https://referencesource.org/state-osha-plan-penalty-maximums/) |
| [Federal Whistleblower Protection Filing Deadlines by Statute](whistleblower-filing-deadlines/) | 25 | 2026-08-15 | [referencesource.org/whistleblower-filing-deadlines/](https://referencesource.org/whistleblower-filing-deadlines/) |
| [How long federal regulations require records to be kept: retention periods, what starts the clock, and who they bind](record-retention-periods-federal/) | 24 | 2026-08-11 | [referencesource.org/record-retention-periods-federal/](https://referencesource.org/record-retention-periods-federal/) |
| [DOT hazmat placarding requirements by hazard class (any-quantity vs. 1,001 lb threshold)](dot-hazmat-placarding-thresholds/) | 23 | 2026-08-19 | [referencesource.org/dot-hazmat-placarding-thresholds/](https://referencesource.org/dot-hazmat-placarding-thresholds/) |
| [Federal incident notification deadlines by regulation](incident-notification-deadlines/) | 23 | 2026-08-12 | [referencesource.org/incident-notification-deadlines/](https://referencesource.org/incident-notification-deadlines/) |
| [OSHA medical surveillance trigger thresholds by substance](osha-medical-surveillance-triggers/) | 23 | 2026-08-12 | [referencesource.org/osha-medical-surveillance-triggers/](https://referencesource.org/osha-medical-surveillance-triggers/) |
| [TLS certificate maximum validity by Certificate Authority: what each CA actually issues today](ca-issuance-validity/) | 22 | 2026-08-18 | [referencesource.org/ca-issuance-validity/](https://referencesource.org/ca-issuance-validity/) |
| [Hydraulic and pipe connection type identification](hydraulic-pipe-connection-types/) | 21 | 2026-08-13 | [referencesource.org/hydraulic-pipe-connection-types/](https://referencesource.org/hydraulic-pipe-connection-types/) |
| [NIST cryptographic algorithm deprecation schedule: what is approved, deprecated, and disallowed, and when](nist-cryptographic-algorithm-deprecation-schedule/) | 21 | 2026-08-16 | [referencesource.org/nist-cryptographic-algorithm-deprecation-schedule/](https://referencesource.org/nist-cryptographic-algorithm-deprecation-schedule/) |
| [State pharmacy technician-to-pharmacist supervision ratios](pharmacy-technician-supervision-ratios/) | 21 | 2026-08-16 | [referencesource.org/pharmacy-technician-supervision-ratios/](https://referencesource.org/pharmacy-technician-supervision-ratios/) |
| [State construction defect statute of limitations and statute of repose periods](state-construction-defect-limitations-periods/) | 20 | 2026-08-18 | [referencesource.org/state-construction-defect-limitations-periods/](https://referencesource.org/state-construction-defect-limitations-periods/) |
| [Dam safety hazard classification, inspection frequency, and owner obligations by US state](state-dam-safety-classification/) | 20 | 2026-08-18 | [referencesource.org/state-dam-safety-classification/](https://referencesource.org/state-dam-safety-classification/) |
| [EPCRA Tier II hazardous chemical inventory reporting thresholds by state](epcra-tier-ii-state-reporting-thresholds/) | 19 | 2026-08-18 | [referencesource.org/epcra-tier-ii-state-reporting-thresholds/](https://referencesource.org/epcra-tier-ii-state-reporting-thresholds/) |
| [US state data breach notification deadlines by state](data-breach-notification-clocks/) | 18 | 2026-08-18 | [referencesource.org/data-breach-notification-clocks/](https://referencesource.org/data-breach-notification-clocks/) |
| [Gift card expiration, fee and cash-redemption rules by state](gift-card-consumer-protections-by-state/) | 18 | 2026-08-18 | [referencesource.org/gift-card-consumer-protections-by-state/](https://referencesource.org/gift-card-consumer-protections-by-state/) |
| [State below-cost motor fuel selling laws and minimum-markup percentages](motor-fuel-minimum-markup-laws-by-state/) | 18 | 2026-08-20 | [referencesource.org/motor-fuel-minimum-markup-laws-by-state/](https://referencesource.org/motor-fuel-minimum-markup-laws-by-state/) |
| [US state consumer data privacy laws: applicability thresholds by state](state-data-privacy-applicability-thresholds/) | 18 | 2026-08-12 | [referencesource.org/state-data-privacy-applicability-thresholds/](https://referencesource.org/state-data-privacy-applicability-thresholds/) |
| [Gas cylinder color codes by standard and country](gas-cylinder-color-codes/) | 17 | 2026-08-05 | [referencesource.org/gas-cylinder-color-codes/](https://referencesource.org/gas-cylinder-color-codes/) |
| [Hazardous waste generator categories — federal vs California vs Washington thresholds and obligations](hazwaste-generator-category-thresholds/) | 17 | 2026-08-11 | [referencesource.org/hazwaste-generator-category-thresholds/](https://referencesource.org/hazwaste-generator-category-thresholds/) |
| [How long medical certificates last for pilots, commercial drivers and merchant mariners — by class, age and service type](medical-certificate-validity-by-occupation/) | 17 | 2026-08-11 | [referencesource.org/medical-certificate-validity-by-occupation/](https://referencesource.org/medical-certificate-validity-by-occupation/) |
| [Workers' compensation waiting periods and retroactive thresholds by US state](wc-waiting-periods-by-state/) | 17 | 2026-08-17 | [referencesource.org/wc-waiting-periods-by-state/](https://referencesource.org/wc-waiting-periods-by-state/) |
| [Toll transponder interoperability: which pass works in which states](toll-transponder-interoperability/) | 16 | 2026-08-19 | [referencesource.org/toll-transponder-interoperability/](https://referencesource.org/toll-transponder-interoperability/) |
| [EPA TSCA Section 6 chemical risk management status: prohibitions, effective dates, and exemptions](tsca-section-6-chemical-risk-management-status/) | 16 | 2026-08-18 | [referencesource.org/tsca-section-6-chemical-risk-management-status/](https://referencesource.org/tsca-section-6-chemical-risk-management-status/) |
| [Electrician licence reciprocity by state: which states accept which licences, in which direction, on what conditions](electrician-licence-reciprocity-by-state/) | 15 | 2026-08-11 | [referencesource.org/electrician-licence-reciprocity-by-state/](https://referencesource.org/electrician-licence-reciprocity-by-state/) |
| [Lithium battery shipping limits (49 CFR 173.185)](lithium-battery-shipping-limits/) | 15 | 2026-08-03 | [referencesource.org/lithium-battery-shipping-limits/](https://referencesource.org/lithium-battery-shipping-limits/) |
| [State controlled-substance scheduling of xylazine and tianeptine](state-emerging-substance-scheduling/) | 15 | 2026-08-19 | [referencesource.org/state-emerging-substance-scheduling/](https://referencesource.org/state-emerging-substance-scheduling/) |
| [State paid family and medical leave program contribution rates, benefits, and eligibility](state-paid-family-leave-programs/) | 15 | 2026-08-17 | [referencesource.org/state-paid-family-leave-programs/](https://referencesource.org/state-paid-family-leave-programs/) |
| [Does this vendor train AI models on your data? Per-product, per-tier, quoted from the current policy](ai-training-data-use-by-vendor/) | 14 | 2026-08-10 | [referencesource.org/ai-training-data-use-by-vendor/](https://referencesource.org/ai-training-data-use-by-vendor/) |
| [Ordering a birth certificate: each state's own fee and process](birth-certificate-fees-by-state/) | 14 | 2026-08-18 | [referencesource.org/birth-certificate-fees-by-state/](https://referencesource.org/birth-certificate-fees-by-state/) |
| [Driver's license point systems: suspension thresholds and lookback periods by US state](driver-license-points-thresholds-by-state/) | 14 | 2026-08-19 | [referencesource.org/driver-license-points-thresholds-by-state/](https://referencesource.org/driver-license-points-thresholds-by-state/) |
| [US state paid family and medical leave (PFML) program requirements for employers](state-paid-family-medical-leave-programs/) | 14 | 2026-08-12 | [referencesource.org/state-paid-family-medical-leave-programs/](https://referencesource.org/state-paid-family-medical-leave-programs/) |
| [State pay transparency laws — salary range disclosure requirements](state-pay-transparency-salary-range-disclosure/) | 14 | 2026-08-19 | [referencesource.org/state-pay-transparency-salary-range-disclosure/](https://referencesource.org/state-pay-transparency-salary-range-disclosure/) |
| [State unemployment insurance taxable wage bases and new employer tax rates by US state](state-ui-taxable-wage-bases/) | 14 | 2026-08-18 | [referencesource.org/state-ui-taxable-wage-bases/](https://referencesource.org/state-ui-taxable-wage-bases/) |
| [Aircraft inspection and test intervals under 14 CFR Part 91](aircraft-inspection-and-test-intervals/) | 13 | 2026-08-06 | [referencesource.org/aircraft-inspection-and-test-intervals/](https://referencesource.org/aircraft-inspection-and-test-intervals/) |
| [Clean Air Act "major source" emission thresholds by pollutant and area classification](clean-air-act-major-source-thresholds/) | 13 | 2026-08-19 | [referencesource.org/clean-air-act-major-source-thresholds/](https://referencesource.org/clean-air-act-major-source-thresholds/) |
| [Competitive bid thresholds for local government by US state — the dollar amount at which a city, county or school district must formally bid, with statutory citations](competitive-bid-thresholds-by-state/) | 13 | 2026-08-19 | [referencesource.org/competitive-bid-thresholds-by-state/](https://referencesource.org/competitive-bid-thresholds-by-state/) |
| [Certificate of Need capital expenditure thresholds by US state — dollar thresholds by facility type, covered services, reviewing agencies, and program status](con-capital-expenditure-thresholds-by-state/) | 13 | 2026-08-19 | [referencesource.org/con-capital-expenditure-thresholds-by-state/](https://referencesource.org/con-capital-expenditure-thresholds-by-state/) |
| [Property tax assessment appeal deadlines by state](property-tax-appeal-deadlines-by-state/) | 13 | 2026-08-25 | [referencesource.org/property-tax-appeal-deadlines-by-state/](https://referencesource.org/property-tax-appeal-deadlines-by-state/) |
| [State small estate affidavit and simplified probate thresholds](state-small-estate-affidavit-thresholds/) | 13 | 2026-08-18 | [referencesource.org/state-small-estate-affidavit-thresholds/](https://referencesource.org/state-small-estate-affidavit-thresholds/) |
| [Vehicle title transfer deadlines and late penalties by state](vehicle-title-transfer-deadlines-by-state/) | 13 | 2026-08-18 | [referencesource.org/vehicle-title-transfer-deadlines-by-state/](https://referencesource.org/vehicle-title-transfer-deadlines-by-state/) |
| [Private well water testing at property sale: which states require it](well-water-testing-at-property-transfer/) | 13 | 2026-08-19 | [referencesource.org/well-water-testing-at-property-transfer/](https://referencesource.org/well-water-testing-at-property-transfer/) |
| [Will execution requirements by state: witnesses, notarization, holographic and electronic wills](will-execution-requirements-by-state/) | 13 | 2026-08-18 | [referencesource.org/will-execution-requirements-by-state/](https://referencesource.org/will-execution-requirements-by-state/) |
| [Reckless / excessive-speeding mph thresholds that trigger a criminal charge, by state](reckless-driving-speed-thresholds-by-state/) | 12 | 2026-08-20 | [referencesource.org/reckless-driving-speed-thresholds-by-state/](https://referencesource.org/reckless-driving-speed-thresholds-by-state/) |
| [State lemon law eligibility thresholds: time limits, mileage, and repair attempts by US state](state-lemon-law-eligibility-thresholds/) | 12 | 2026-08-17 | [referencesource.org/state-lemon-law-eligibility-thresholds/](https://referencesource.org/state-lemon-law-eligibility-thresholds/) |
| [Thermocouple type letter to alloy pair, ANSI/IEC color code and tolerance class](thermocouple-type-color-code-crosswalk/) | 12 | 2026-08-19 | [referencesource.org/thermocouple-type-color-code-crosswalk/](https://referencesource.org/thermocouple-type-color-code-crosswalk/) |
| [General contractor license requirements and dollar thresholds by US state](general-contractor-license-thresholds-by-state/) | 11 | 2026-08-17 | [referencesource.org/general-contractor-license-thresholds-by-state/](https://referencesource.org/general-contractor-license-thresholds-by-state/) |
| [Recreational boat safety equipment requirements by vessel length](recreational-boat-safety-equipment-requirements-by-length/) | 11 | 2026-08-25 | [referencesource.org/recreational-boat-safety-equipment-requirements-by-length/](https://referencesource.org/recreational-boat-safety-equipment-requirements-by-length/) |
| [State Earned Wage Access (EWA) Regulatory Frameworks — Classification, Fee Caps, and Licensing Requirements](state-earned-wage-access-regulations/) | 11 | 2026-08-18 | [referencesource.org/state-earned-wage-access-regulations/](https://referencesource.org/state-earned-wage-access-regulations/) |
| [State mini-WARN act thresholds: layoff notice requirements beyond federal WARN](state-mini-warn-act-thresholds/) | 11 | 2026-08-18 | [referencesource.org/state-mini-warn-act-thresholds/](https://referencesource.org/state-mini-warn-act-thresholds/) |
| [State Opioid Initial Prescribing Limits](state-opioid-prescribing-limits/) | 11 | 2026-08-18 | [referencesource.org/state-opioid-prescribing-limits/](https://referencesource.org/state-opioid-prescribing-limits/) |
| [State prevailing wage law applicability thresholds](state-prevailing-wage-thresholds/) | 11 | 2026-08-15 | [referencesource.org/state-prevailing-wage-thresholds/](https://referencesource.org/state-prevailing-wage-thresholds/) |
| [State drug price transparency reporting thresholds, triggers, and penalties for pharmaceutical manufacturers](drug-price-transparency-thresholds/) | 10 | 2026-08-15 | [referencesource.org/drug-price-transparency-thresholds/](https://referencesource.org/drug-price-transparency-thresholds/) |
| [US state universal occupational license recognition laws — conditions and scope](state-universal-license-recognition-laws/) | 10 | 2026-08-15 | [referencesource.org/state-universal-license-recognition-laws/](https://referencesource.org/state-universal-license-recognition-laws/) |
| [State Worker Classification Tests — Independent Contractor vs Employee](state-worker-classification-tests/) | 10 | 2026-08-18 | [referencesource.org/state-worker-classification-tests/](https://referencesource.org/state-worker-classification-tests/) |
| [Winter utility shutoff/disconnection moratorium by state](utility-shutoff-moratorium-by-state/) | 10 | 2026-08-19 | [referencesource.org/utility-shutoff-moratorium-by-state/](https://referencesource.org/utility-shutoff-moratorium-by-state/) |
| [Miele vacuum cleaner bag type by model series](vacuum-filter-fitment/) | 10 | 2026-08-03 | [referencesource.org/vacuum-filter-fitment/](https://referencesource.org/vacuum-filter-fitment/) |
| [Wage garnishment limits and exempt earnings by state](wage-garnishment-exemption-thresholds-by-state/) | 10 | 2026-08-26 | [referencesource.org/wage-garnishment-exemption-thresholds-by-state/](https://referencesource.org/wage-garnishment-exemption-thresholds-by-state/) |
| [Which energy code each US state enforces for new homes: the IECC edition (or state equivalent) actually in force, with effective dates and amendments, from the state rules themselves](energy-code-adoption-by-state/) | 9 | 2026-08-18 | [referencesource.org/energy-code-adoption-by-state/](https://referencesource.org/energy-code-adoption-by-state/) |
| [FLSA overtime exemption duties tests by category (29 CFR Part 541)](flsa-overtime-exemption-duties-tests/) | 9 | 2026-08-19 | [referencesource.org/flsa-overtime-exemption-duties-tests/](https://referencesource.org/flsa-overtime-exemption-duties-tests/) |
| [Stolen EBT/SNAP benefit replacement policy by US state](stolen-ebt-benefit-replacement-by-state/) | 9 | 2026-08-18 | [referencesource.org/stolen-ebt-benefit-replacement-by-state/](https://referencesource.org/stolen-ebt-benefit-replacement-by-state/) |
| [State Property Tax Exemptions for Disabled Veterans — Exemption Amounts, Disability Rating Thresholds, and Eligibility Rules](veteran-property-tax-exemptions-by-state/) | 9 | 2026-08-18 | [referencesource.org/veteran-property-tax-exemptions-by-state/](https://referencesource.org/veteran-property-tax-exemptions-by-state/) |
| [Building Energy Benchmarking and Performance Standard Requirements by Jurisdiction](building-energy-benchmarking-requirements/) | 8 | 2026-08-15 | [referencesource.org/building-energy-benchmarking-requirements/](https://referencesource.org/building-energy-benchmarking-requirements/) |
| [Life insurance premium grace periods and lapse protections by US state](life-insurance-grace-periods-by-state/) | 8 | 2026-08-17 | [referencesource.org/life-insurance-grace-periods-by-state/](https://referencesource.org/life-insurance-grace-periods-by-state/) |
| [Asbestos Abatement Notification Requirements, Thresholds, and Fees by State](asbestos-notification-requirements-by-state/) | 7 | 2026-08-15 | [referencesource.org/asbestos-notification-requirements-by-state/](https://referencesource.org/asbestos-notification-requirements-by-state/) |
| [Building permit expiry, progress and renewal rules by jurisdiction](building-permit-validity-and-renewal/) | 7 | 2026-08-11 | [referencesource.org/building-permit-validity-and-renewal/](https://referencesource.org/building-permit-validity-and-renewal/) |
| [Catalytic converter sale and possession laws by US state — who can legally buy a used converter, and what a seller must prove](catalytic-converter-theft-laws-by-state/) | 7 | 2026-08-19 | [referencesource.org/catalytic-converter-theft-laws-by-state/](https://referencesource.org/catalytic-converter-theft-laws-by-state/) |
| [DOT minimum random drug and alcohol testing rates by transportation mode](dot-random-drug-alcohol-testing-rates-by-mode/) | 7 | 2026-08-19 | [referencesource.org/dot-random-drug-alcohol-testing-rates-by-mode/](https://referencesource.org/dot-random-drug-alcohol-testing-rates-by-mode/) |
| [Septic system inspection at property sale: which states require it](septic-inspection-at-property-transfer/) | 7 | 2026-08-18 | [referencesource.org/septic-inspection-at-property-transfer/](https://referencesource.org/septic-inspection-at-property-transfer/) |
| [State Heat Illness Prevention Standards — Temperature Triggers and Required Employer Actions](state-heat-illness-prevention-standards/) | 7 | 2026-08-17 | [referencesource.org/state-heat-illness-prevention-standards/](https://referencesource.org/state-heat-illness-prevention-standards/) |
| [Short-term rental registration rules, city by city, from each city's own page](str-registration-rules-major-cities/) | 7 | 2026-08-18 | [referencesource.org/str-registration-rules-major-cities/](https://referencesource.org/str-registration-rules-major-cities/) |
| [Underground Storage Tank Operator Training Requirements by State](ust-operator-training-requirements/) | 7 | 2026-08-18 | [referencesource.org/ust-operator-training-requirements/](https://referencesource.org/ust-operator-training-requirements/) |
| [Workers' compensation insurance requirements by US state: employee thresholds, who counts, and industry exceptions](workers-comp-coverage-thresholds-by-state/) | 7 | 2026-08-12 | [referencesource.org/workers-comp-coverage-thresholds-by-state/](https://referencesource.org/workers-comp-coverage-thresholds-by-state/) |
| [NFA firearm category definitions and current transfer/making tax](nfa-firearm-category-definitions-and-transfer-tax/) | 6 | 2026-08-25 | [referencesource.org/nfa-firearm-category-definitions-and-transfer-tax/](https://referencesource.org/nfa-firearm-category-definitions-and-transfer-tax/) |
| [State Right-to-Repair Laws: Coverage, Requirements, and Effective Dates](state-right-to-repair-laws/) | 6 | 2026-08-15 | [referencesource.org/state-right-to-repair-laws/](https://referencesource.org/state-right-to-repair-laws/) |
| [Unemployment insurance: maximum weekly benefit and weeks of duration by US state](ui-weekly-benefit-and-duration-by-state/) | 6 | 2026-08-18 | [referencesource.org/ui-weekly-benefit-and-duration-by-state/](https://referencesource.org/ui-weekly-benefit-and-duration-by-state/) |
| [Workers' compensation medical fee schedule conversion factors by US state — reimbursement rates, service category breakdowns, fee schedule basis, and effective dates](wc-medical-fee-schedule-multipliers-by-state/) | 6 | 2026-08-18 | [referencesource.org/wc-medical-fee-schedule-multipliers-by-state/](https://referencesource.org/wc-medical-fee-schedule-multipliers-by-state/) |
| [How often gas pumps and retail scales get inspected, by state](weights-measures-device-inspection-intervals-by-state/) | 6 | 2026-08-20 | [referencesource.org/weights-measures-device-inspection-intervals-by-state/](https://referencesource.org/weights-measures-device-inspection-intervals-by-state/) |
| [CDL endorsement prerequisites and testing sequence](cdl-endorsement-prerequisites/) | 5 | 2026-08-19 | [referencesource.org/cdl-endorsement-prerequisites/](https://referencesource.org/cdl-endorsement-prerequisites/) |
| [How often elevators must be inspected in each US state: intervals, filing rules, fees and the ASME A17.1 edition enforced](elevator-inspection-requirements-by-state/) | 5 | 2026-08-11 | [referencesource.org/elevator-inspection-requirements-by-state/](https://referencesource.org/elevator-inspection-requirements-by-state/) |
| [State life and health insurance guaranty association benefit limits — how much is protected if your insurer fails](insurance-guaranty-association-limits-by-state/) | 5 | 2026-08-19 | [referencesource.org/insurance-guaranty-association-limits-by-state/](https://referencesource.org/insurance-guaranty-association-limits-by-state/) |
| [State tuition-free college (promise) programs: eligibility rules by state](state-promise-free-college-programs/) | 5 | 2026-08-18 | [referencesource.org/state-promise-free-college-programs/](https://referencesource.org/state-promise-free-college-programs/) |
| [Maximum legal vehicle size and weight limits by US state](truck-size-weight-limits-by-state/) | 5 | 2026-08-18 | [referencesource.org/truck-size-weight-limits-by-state/](https://referencesource.org/truck-size-weight-limits-by-state/) |
| [Deer hunting season dates by state, 2026–27: archery, firearm and muzzleloader seasons from state wildlife agencies](deer-season-dates-by-state/) | 4 | 2026-08-11 | [referencesource.org/deer-season-dates-by-state/](https://referencesource.org/deer-season-dates-by-state/) |
| [National Electrical Code edition adopted by each US state](nec-adoption-by-state/) | 4 | 2026-08-18 | [referencesource.org/nec-adoption-by-state/](https://referencesource.org/nec-adoption-by-state/) |
| [Which National Electrical Code edition each US state enforces: adoption status, effective dates and amendments, from the state boards themselves](nec-edition-adoption-by-state/) | 4 | 2026-08-11 | [referencesource.org/nec-edition-adoption-by-state/](https://referencesource.org/nec-edition-adoption-by-state/) |
| [NFPA 704 fire diamond ratings by chemical](nfpa-704-hazard-ratings/) | 4 | 2026-08-06 | [referencesource.org/nfpa-704-hazard-ratings/](https://referencesource.org/nfpa-704-hazard-ratings/) |
| [GIS vector format capabilities and limitations in GDAL](file-format-software-version-compatibility/) | 3 | 2026-08-04 | [referencesource.org/file-format-software-version-compatibility/](https://referencesource.org/file-format-software-version-compatibility/) |
| [Intrastate truck driver hours-of-service rules by state — where they differ from federal](intrastate-driver-hours-by-state/) | 3 | 2026-08-11 | [referencesource.org/intrastate-driver-hours-by-state/](https://referencesource.org/intrastate-driver-hours-by-state/) |
| [Electrician licence progression: training hours and prerequisites by US state](electrician-licence-progression-by-state/) | 2 | 2026-08-06 | [referencesource.org/electrician-licence-progression-by-state/](https://referencesource.org/electrician-licence-progression-by-state/) |
