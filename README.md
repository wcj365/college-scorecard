# College Scorecard Data Exploration

## References
- https://community.tibco.com/wiki/college-scorecard-analysis
- https://homes.cs.washington.edu/~jheer/
- https://nextjournal.com/sdanisch/data-types-graphical-marks-and-visual-encoding-channels#summary
- https://courses.cs.washington.edu/courses/cse512/19sp/

## Data Elements for Analysis
The data file contains many columns. Only load the columns of interest. 
- __UNITID__ <br>Data files are provided at the UNITID level, which is the unique identification number assigned to postsecondary institutions as surveyed through IPEDS - Integrated Postsecondary Education Data System.


- __INSTNM__ <br>The institution’s name, as reported in IPEDS.


- __CITY, STABBR__ <br>City and State abbreviation As reported in IPEDS.


- __NUMBRANCH__ <br>This variable identifies the number of branch campuses at that institution.


- __HIGHDEG__ <br>Highest award identifies the highest award level conferred at the institution.


- __PREDDEG__ <br>Predominant undergraduate award identifies the type of award that the institution primarily confers; for instance, an institution that awards 40 percent bachelor’s degrees, 30 percent associate degrees, and 30 percent certificate programs would be classified as predominantly bachelor’s degree awarding.


- __CONTROL__ <br>This element is reported directly to IPEDS, and identifies whether the institution’s governance structure is public, private nonprofit, or private for-profit.


- __DISTANCEONLY__ <br>Institutions are identified as distance education-only if all their programs are available only via distance education.


- __TUITFTE__ <br>The net tuition revenue per full-time equivalent (FTE) student uses tuition revenue minus discounts and allowances, and divides that by the number of FTE undergraduate and graduate students.


- __AVGFACSAL__ <br>The average faculty salary produces the average faculty salary per month, by dividing the total salary outlays by the number of months worked for all full-time, nonmedical instructional staff.


- __ADM_RATE_ALL__ <br>Colleges report to IPEDS their Fall admissions rate, defined as the number of admitted undergraduates divided by the number of undergraduates who applied. ADM_RATE_ALL represents the admissions rate across all campuses, defined as the total number of admitted undergraduates across all branches divided by the total number of undergraduates who applied across all branches.


- __SATVR25, SATVR75, SATMT25, SATMT75, ACTCM25, ACTCM75__ <br>The files include the 25th and 75th percentiles of SAT reading (SATVR* for _25 and _75), writing (SATWR* for _25 and _75), math (SATMT* for _25 and _75) <br> NOTE: Data for SATWR is absent and the corresponding columns should be dropped.


- __UGDS__ <br>This element includes the number of degree/certificate-seeking undergraduates enrolled in the fall, as reported in the IPEDS Fall Enrollment component.


- __UG25ABV__ <br>This element identifies the share of students enrolled as of the institutions official fall census date (or October 15 of the IPEDS collection year, whichever is earlier) who are ages 25 and over.


- __PCTFLOAN__ <br>This element, as reported in the IPEDS Student Financial Aid (SFA) component, shows the share of undergraduate students who received federal loans in a given year.


- __CDR3__ <br>Cohort default rates are produced annually as an institutional accountability metric; institutions with high default rates may lose access to federal financial aid. The three-year cohort default rate (CDR3) represents a snapshot in time.

- __PAR_ED_PCT_1STGEN__ <br>percent 1st gen students.

- __MD_EARN_WNE_P6__ <br>median earnings, 6 years after graduation.

Data Mapping per Documentatoin:

#### Degrees (HIGHDGE, PREDDGE)
- 4 : Graduate's Degree
- 3 : Bachelor's Degree
- 2 : Associate's Degree
- 1 : Certificate
- 0 : N/A

#### Institution Type (CONTROL)
- 1 : Public
- 2 : Private Nonprofit
- 3 : Private For-Profit

#### Distance Learning Only (DISTANCEONLY)
- 0 : No
- 1 : Yes
