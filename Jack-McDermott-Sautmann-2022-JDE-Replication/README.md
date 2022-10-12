Instructions for working with data and dofiles for Jack, McDermott and Sautmann “Multiple Price Lists for Willingness to Pay Elicitation” (referred to below as JMS).

The implementation package for data collection, data cleaning and data analysis to carry out willingness-to-pay measurement using an MPL are provided in a separate GitHub repository: https://github.com/MPL-WTP/MPL-WTP. The data and code provided for replication reproduces Tables 2, 3 and A.1 and Figures 3 and 4 in the published manuscript.

### Data
Two files are included for replication, in Stata format. They provide alternative transformations of the data collected using the MPL survey instrument coded in SurveyCTO. The data cleaning and formatting largely followed the description in the Appendix and the scripts provided on GitHub.

- JMS-SA_data_mplwtp.dta contains the reshaped data to generate Tables 2 and A.1 and implement the estimation strategy described in JMS.
- JMS-SA_data_intervalreg.dta contains the same data, set up for interval regression, used to generate Table 3 and Figures 3 and 4.

### Code
The replication script is provided in MPL_SA_do.do. It implements the regressions underlying the tables and figures in the manuscript. It also calls two user-written ado files: mplwtp.ado and mplwtp_xtset.ado. The latter is not used for the tables produced in JMS but is required to implement the bootstrapped standard errors option in mplwtp, and so is provided for completeness. Additional discussion is available in the technical appendix and GitHub repo.  
