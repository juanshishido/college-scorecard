# Ideas, Considerations, and Variables

## Description of the data

*Yearly* information on thousands of colleges and universities in the United
States. Enrollment rates, financial aid, loans, debts, etc. Some of this data
is from the IRS. Information is provided for both four-year institutions and
for community colleges.

**Important**:

* It *only* includes data for students accepting federal aid. This
  differs greatly by institution.
* Also, "typical total debt" only includes federal loans. It does not, for
  example, include Parent Plus or other non-federal loans.
* Be careful in comparing graduation rates for community colleges. Figure out
  how they calculate those statistics. Perhaps, analyze by institution type.
    * **How** does (do they even?) the College Scorecard track individuals who
      went to a community college and then transferred to a four-year
      institution?
* There are some universities from Puerto Rico.

## Potential ideas

1. What's the relationship between federal tax credits and grants and the
   amount that schools offer. This is on a yearly basis.

    * Can we predict average financial aid amounts?

**Concerns**

* Limited number of years of data

2. What affects financial aid? Of course, there are state budgets, enrollments,
   federal funds, donations, grants, etc.

    * Can we identify factors that increase awarded aid?

**Concerns**

* There may be student differences both across schools and across times in
  terms of propensity to accept. Are the numbers relfected the "awarded"
  amounts or are they the accepted amounts? Control for attendance costs

3. Can we see differences in graduation rates across time?

4. What's the relationship between "highly ranked" schools and financial aid
   awarded? And the relationship with cost?

5. Which schools provide the "biggest bang for your buck?"

6. Are we able to tell the proportion of students who received federal
   financial aid with this data?

    * It seems possible according to
      [this](http://www.readingeagle.com/news/article/crunching-college-data-college-scorecard-gets-graded-by-berks-universities)
      (for some reason, the link itself doesn't work; it only works when
      referred by Google).

7. What can we extract from the average monthly payment figure?

8. There is information on "college's initial cost." These figures are broken
   down by family income bracket.

9. How do majors affect outcomes?

    * Could we predict income based on majors?

10. How do grants, loans, and defaults interact?

11. In what parts of the country do students *accept* loans the most? Default
    the most?

# Variables of Interest

* `UNITID`
* `OPEID`
* `INSTNM`
* `CITY`
* `sch_deg`
* `main`
* `PREDDEG`
* `HIGHDEG`
* `CONTROL`
* `ADM_RATE`
* `SAT`...
* `PCIP`&mdash;but aggregate categories
* `DISTANCEONLY`
* `UGDS`
* `UGDS_`race&mdash;only available for 2008-2013
* `NPT4_PUB`&mdash;only available for 2009-2013
* `NPT4_PRIV`&mdash;only available for 2009-2013
* `NPT41_PUB` - `NPT45_PUB`
* `NPT41_PRIV` - `NPT45_PRIV`
* `NUM4_PUB`
* `NUM4_PRIV`
* `NUM41_PUB` - `NUM45_PUB`
* `NUM41_PRIV` - `NUM41_PRIV`
* `COSTT4_A`&mdash;only available for 2009-2013
* `COSTT4_P`&mdash;only available for 2009-2013
* `TUITIONFEE_IN`&mdash;only available for 2000-2013
* `TUITIONFEE_OUT`&mdash;only available for 2000-2013
* `TUITFTE`&mdash;only available for 1998-2013
* `INEXPFTE`&mdash;only available for 1998-2013
* `AVGFACSAL`&mdash;missing for year 2000
* `PCTPELL`&mdash;only available for 2008-2013
