# Analysis-of-Covid19
Analyzing covid cases recorded in the USA.

### Columns in the Dataset

| Column Name | Description | Type |
| ----------- | ----------- | ---- |
|cdc_case_earliest_dt | The earlier of the Clinical Date (date related to the illness or specimen collection) or the Date Received by CDC. Calculated date-- Cdc_case_earliest_dt uses the best available date from the set of dates related to illness/specimen collection and the set of dates related to when a case is reported. It is an option to end-users who need a date variable with optimized completeness. The logic of cdc_case_earliest_dt is to use the non-null date of one variable when the other is null and to use the earliest valid date when both dates are available. If no date available, then left blank. | Date & Time |
| cdc_report_dt | Date case was first reported to the CDC. Calculated date-- Depreciated; CDC recommends researchers use cdc_case_earliest_dt in time series and other analyses. This date was populated using the date at which a case record was first submitted to the database. If missing, then the report date entered on the case report form was used. If missing, then the date at which the case first appeared in the database was used. If none available, then left blank. | Date & Time |
| pos_spec_dt | Date of first positive specimen collection (Case Report Form) | Date & Time |
| onset_dt | Symptom onset date, if symptomatic (Case Report Form) | Date & Time |
| current_status | Case Status (Case Report Form: What is the current status of this person?) -- Values: Laboratory-confirmed case; Probable case; Please see latest CSTE case definition for more information. | Plain Text |
| sex | Sex (Case Report Form): Male; Female; Unknown; Other; Missing; NA | Plain Text |
| age_group | Age Group: 0 - 9 Years; 10 - 19 Years; 20 - 39 Years; 40 - 49 Years; 50 - 59 Years; 60 - 69 Years; 70 - 79 Years; 80 + Years; Missing; NA; The age group categorizations were populated using the age value that was reported on the case report form. Date of birth was used to fill in missing/unknown age values using the difference in time between date of birth and onset date. | Plain Text |
| race_ethnicity_combined | Race and ethnicity (combined): American Indian/Alaska Native, Non-Hispanic; Asian, Non-Hispanic; Black, Non-Hispanic; Multiple/Other, Non-Hispanic; Native Hawaiian/Other Pacific Islander, Non-Hispanic; White, Non-Hispanic; Hispanic/Latino; Unknown; Missing; NA. If more than race was reported, race was categorized into multiple/other races. | Plain Text |
| hosp_yn | Hospitalization status (Case Report Form: Was the patient hospitalized?) -- Values: Yes; No; Unknown; Missing; | Plain Text |
| icu_yn | ICU admission status (Case Report Form: Was the patient admitted to an intensive care unit (ICU)?) -- Values: Yes; No; Unknown; Missing; | Plain Text |
| death_yn | Death status (Case Report Form: Did the patient die as a result of this illness?) -- Values: Yes; No; Unknown; Missing; | Plain Text |
| medcond_yn | Presence of underlying comorbidity or disease (Case Report Form: Pre-existing medical conditions?) -- Values: Yes; No; Unknown; Missing; | Plain Text |

