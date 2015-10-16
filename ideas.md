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
* `COMP_ORIG_YR4_RT` &mdash; available for 2000-2012
* `WDRAW_ORIG_YR4_RT` &mdash; available for 2000-2012
* `ENRL_ORIG_YR4_RT` &mdash; available for 2000-2012
* `LO_INC_COMP_ORIG_YR4_RT` &mdash; available for 2000-2012
* `LO_INC_WDRAW_ORIG_YR4_RT` &mdash; available for 2000-2012
* `MD_INC_COMP_ORIG_YR4_RT` &mdash; available for 2000-2012
* `MD_INC_WDRAW_ORIG_YR4_RT` &mdash; available for 2000-2012
* `HI_INC_COMP_ORIG_YR4_RT` &mdash; available for 2000-2012
* `HI_INC_WDRAW_ORIG_YR4_RT` &mdash; available for 2000-2012
* `DEP_COMP_ORIG_YR4_RT` &mdash; available for 2000-2012
* `DEP_WDRAW_ORIG_YR4_RT` &mdash; available for 2000-2012
* `IND_COMP_ORIG_YR4_RT` &mdash; available for 2000-2012
* `IND_WDRAW_ORIG_YR4_RT` &mdash; available for 2000-2012
* `COMPL_RPY_1YR_RT` &mdash; available for 2000-2012
* `NONCOM_RPY_1YR_RT` &mdash; available for 2007-2011
* `LO_INC_RPY_1YR_RT` &mdash; available for 2007-2011
* `MD_INC_RPY_1YR_RT` &mdash; available for 2007-2011
* `HI_INC_RPY_1YR_RT` &mdash; available for 2007-2011
* `DEP_RPY_1YR_RT` &mdash; available for 2007-2011
* `IND_RPY_1YR_RT` &mdash; available for 2007-2011
* `COMPL_RPY_3YR_RT` &mdash; available for 2009-2013
* `NONCOM_RPY_3YR_RT` &mdash; available for 2009-2013
* `LO_INC_RPY_3YR_RT` &mdash; available for 2009-2013
* `MD_INC_RPY_3YR_RT` &mdash; available for 2009-2013
* `HI_INC_RPY_3YR_RT` &mdash; available for 2009-2013
* `DEP_RPY_3YR_RT` &mdash; available for 2009-2013
* `IND_RPY_3YR_RT` &mdash; available for 2009-2013
* `COMPL_RPY_5YR_RT` &mdash; available for 2011-2013
* `NONCOM_RPY_5YR_RT` &mdash; available for 2011-2013
* `LO_INC_RPY_5YR_RT` &mdash; available for 2011-2013
* `MD_INC_RPY_5YR_RT` &mdash; available for 2011-2013
* `HI_INC_RPY_5YR_RT` &mdash; available for 2011-2013
* `DEP_RPY_5YR_RT` &mdash; available for 2011-2013
* `IND_RPY_5YR_RT` &mdash; available for 2011-2013
* `COMPL_RPY_7YR_RT` &mdash; available for 2013
* `NONCOM_RPY_7YR_RT` &mdash; available for 2013
* `LO_INC_RPY_7YR_RT` &mdash; available for 2013
* `MD_INC_RPY_7YR_RT` &mdash; available for 2013
* `HI_INC_RPY_7YR_RT` &mdash; available for 2013
* `DEP_RPY_7YR_RT` &mdash; available for 2013
* `IND_RPY_7YR_RT` &mdash; available for 2013
* `GRAD_DEBT_MDN` &mdash; available for 1997-2013
* `WDRAW_DEBT_MDN` &mdash; available for 1997-2013
* `LO_INC_DEBT_MDN` &mdash; available for 1997-2013
* `MD_INC_DEBT_MDN` &mdash; available for 1997-2013
* `HI_INC_DEBT_MDN` &mdash; available for 1997-2013
* ***Could potentially include those with Pell grants vs. those W/O. Would need to include in repayment data***
* `CUML_DEBT_N` &mdash; available for 1997-2013
* `CUML_DEBT_P90` &mdash; available for 1997-2013
* `CUML_DEBT_P75` &mdash; available for 1997-2013
* `CUML_DEBT_P25` &mdash; available for 1997-2013
* `CUML_DEBT_P10` &mdash; available for 1997-2013
* `HCM2` &mdash; available for 1996-2013
* `count_nwne_p10` &mdash; available for 2007, 2009, 2011
* `count_wne_p10` &mdash; available for 2007, 2009, 2011
* `mn_earn_wne_p10` &mdash; available for 2007, 2009, 2011
* `md_earn_wne_p10` &mdash; available for 2007, 2009, 2011
* `pct10_earn_wne_p10` &mdash; available for 2007, 2009, 2011
* `pct25_earn_wne_p10` &mdash; available for 2007, 2009, 2011
* `pct75_earn_wne_p10` &mdash; available for 2007, 2009, 2011
* `pct90_earn_wne_p10` &mdash; available for 2007, 2009, 2011
* `sd_earn_wne_p10` &mdash; available for 2007, 2009, 2011
* `count_wne_inc1_p10` &mdash; available for 2007, 2009, 2011
* `count_wne_inc2_p10` &mdash; available for 2007, 2009, 2011
* `count_wne_inc3_p10` &mdash; available for 2007, 2009, 2011
* `mn_earn_wne_inc1_p10` &mdash; available for 2007, 2009, 2011
* `mn_earn_wne_inc2_p10` &mdash; available for 2007, 2009, 2011
* `mn_earn_wne_inc3_p10` &mdash; available for 2007, 2009, 2011
* `count_nwne_p6` &mdash; available for 2003, 2005, 2007, 2009, 2011
* `count_wne_p6` &mdash; available for 2003, 2005, 2007, 2009, 2011
* `mn_earn_wne_p6` &mdash; available for 2003, 2005, 2007, 2009, 2011
* `md_earn_wne_p6` &mdash; available for 2003, 2005, 2007, 2009, 2011
* `pct10_earn_wne_p6` &mdash; available for 2003, 2005, 2007, 2009, 2011
* `pct25_earn_wne_p6` &mdash; available for 2003, 2005, 2007, 2009, 2011
* `pct75_earn_wne_p6` &mdash; available for 2003, 2005, 2007, 2009, 2011
* `pct90_earn_wne_p6` &mdash; available for 2003, 2005, 2007, 2009, 2011
* `sd_earn_wne_p6` &mdash; available for 2003, 2005, 2007, 2009, 2011
* `count_wne_inc1_p6` &mdash; available for 2003, 2005, 2007, 2009, 2011
* `count_wne_inc2_p6` &mdash; available for 2003, 2005, 2007, 2009, 2011
* `count_wne_inc3_p6` &mdash; available for 2003, 2005, 2007, 2009, 2011
* `DEBT_MDN_SUPP` &mdash; available for 1997-2013
* `mn_earn_wne_inc1_p6` &mdash; available for 2003, 2005, 2007, 2009, 2011
* `mn_earn_wne_inc2_p6` &mdash; available for 2003, 2005, 2007, 2009, 2011
* `mn_earn_wne_inc3_p6` &mdash; available for 2003, 2005, 2007, 2009, 2011