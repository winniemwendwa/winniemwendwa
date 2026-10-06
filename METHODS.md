# Methods and interpretation

Source: user-supplied CA YR4 RESULTS.xlsx, Sheet1; 219 nonempty records and 350 columns. These are survey records, not independently verified unique households. All records were retained; no duplicate submission UUIDs were found. Survey dates come from the start field. Respondent gender is distinct from household head gender and household type.

## Denominators
Yes/no indicators use recognised yes/no responses. All-three-principles adoption is 160/209 among respondents answering that question, and 160/219 (73.1%) using the full survey sample. The conditional percentage is not the full-sample adoption rate. Individual practice rates use valid binary responses among the 209 reporting CA principles; the survey's branching is preserved, not silently recoded.

## Yield calculations
Only records reporting that the crop was grown qualify. Maize, sorghum, and millet also require a yes response to their harvested question. Cowpeas and green grams have no equivalent harvested-status field in the mapped schema. Require finite positive area and finite nonnegative harvest. Record-level yield = kilograms / acres. Main result = arithmetic mean of eligible record-level yields; zero harvest is retained where area is positive. Also show median, number of valid records, positive-harvest-only mean, and area-weighted yield = sum(kg)/sum(acres). Means excluding zero harvest describe successful harvests and can overstate overall production performance; they are a separately labelled alternative.

Four CF crop-area observations exceed 20 acres, with maxima of 810 (cowpeas), 600 (green grams), 90 (sorghum), and 100 (millet). These values may reflect entry or unit issues but are not corrected without confirmation. The primary tables retain them. A sensitivity mean excludes area above 20 acres for illustration; 20 is an analyst screening threshold, not a validated agronomic cutoff. Area-weighted estimates are particularly sensitive to these entries. Do not treat the portfolio's CA-CF contrasts as validated impact estimates.

CA and CF groups have unequal sample sizes and may overlap within households. No matching, significance test, seasonal adjustment, or causal identification is claimed. Results are descriptive and unweighted. No baseline or target values are present in this workbook, so this portfolio does not fabricate baseline/target comparisons.

## Food provision
Adequate-food months = 12 minus the stored total months without adequate food. Accept integer totals from 0 to 12, retaining zero. All 219 totals meet this check, and the stored adequate-month field agrees. The food questions mix “past 12 months” and “past 6 months,” and their month labels span inconsistent years. Thus the 10.37-month average and 58.9% full-year adequacy are provisional indicators based on recorded totals; confirm recall-period wording before formal reporting. No monthly trend is published.

## Quality checks
Nine records differ between the CA-practice yes/no question and the CA-principles yes/no question. Treat these as different survey items and review them rather than merging their counts. UUID checks establish submission duplication only, not unique-household identity. This public package contains only aggregate results, charts, methods, and code. Names, GPS, identifiers, exact timestamps, free text, interviewer details, and row-level household data are excluded.

## Attribution
This portfolio was prepared for Winnie K. from her supplied project dataset with AI-assisted analysis and documentation. It demonstrates an analysis workflow; it does not independently establish who collected the data, authored original project outputs, or caused programme outcomes. Only claim professional roles and achievements you can substantiate.
