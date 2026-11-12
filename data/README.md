# Data

`working_time.csv` contains course calculations from the
[2024 American Time Use Survey](https://www.bls.gov/tus/data/datafiles-2024.htm),
US Bureau of Labor Statistics. The source was located through
[Todd Jones's dataset catalogue](https://github.com/toddrjones/datasets).

The sample comprises 2,762 one-day diaries from employed US adults aged 25-54,
including part-time workers and people absent from work. Diaries with zero time
in an activity are retained. Estimates use survey weights and are not adjusted
for differences in jobs or household circumstances.

| Column | Definition |
| --- | --- |
| `day_type` | Weekdays, or weekends and holidays. Holidays are grouped with weekends regardless of the day of the week. |
| `measure` | Job-related work, household and care work, or combined work; defined below. |
| `series` | Men, Women, or Women minus men. Men and Women are averages for the survey's male/female sex categories; Women minus men is their difference. |
| `estimate_hours` | Estimated hours per person per day, or the difference in those hours. |
| `ci_low_hours` | Lower endpoint of the estimate's 95% confidence interval. |
| `ci_high_hours` | Upper endpoint of the estimate's 95% confidence interval. |

**Job-related work** includes working, work-related activities and their travel
(ATUS codes 0501, 0502, 180501 and 180502). **Household and care work** includes
household tasks and caring for or helping household and non-household members,
with related travel (02, 03, 04, 1802, 1803 and 1804). **Combined work** is their sum.
These are primary activities; simultaneous secondary care is not counted.
Shopping, volunteering and job search are outside these measures.

The 18 rows are estimates, not individual records. Intervals are pointwise 95%
normal-approximation confidence intervals, calculated using the 160 BLS replicate
weights. Combined-work and difference intervals were calculated directly from
their replicate estimates. See the [ATUS User's Guide, section 7.5](https://www.bls.gov/tus/atususersguide.pdf)
and [2024 activity definitions](https://www.bls.gov/tus/lexicons/lexiconnoex2024.pdf).

BLS data are [public domain](https://www.bls.gov/bls/linksite.htm).
