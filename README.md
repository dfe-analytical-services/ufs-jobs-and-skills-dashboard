# ufs-jobs-and-skills-dashboard
Dashboard from the Unit for Future Skills covering jobs and skills

## Introduction 

Give a brief overview of what your app is for here. 

Add links to where each version of your app is deployed - e.g.

- Production - https://rsconnect/rsc/dfe-published-data-qa
- Pre-production - https://rsconnect-pp/rsc/dfe-published-data-qa
- Development - https://rsconnect-pp/rsc/dev-dfe-published-data-qa


---

## Requirements

You should list out the software and programming skills needed, as well as any access requirements e.g.


### i. Software requirements (for running locally)

- Installation of R Studio 1.2.5033 or higher

- Installation of R 3.6.2 or higher

- Installation of RTools40 or higher

### ii. Programming skills required (for editing or troubleshooting)

- R at an intermediate level, [DfE R training guide](https://dfe-analytical-services.github.io/r-training-course/)

- Particularly [R Shiny](https://shiny.rstudio.com/)

### iii. Access requirements

- Access to the Stats Development Team SQL modelling area (MA_SDT_NS_DATA) in T1PRANMSQL\SQLPROD,60125. Request access from Cam Race and forward on your request to the PDR mailbox (PupilData.REPOSITORY@education.gov.uk)
  
---

## How to use

You should clearly lay out the steps needed to run your code here - generally, they will be similar to the below for Shiny apps:


### Running the app locally

1. Clone or download the repo. 

2. Open the R project in R Studio.

3. Run `renv::restore()` to install dependencies.

4. Run `shiny::runApp()` to run the app locally.


### Packages

Package control is handled using renv. As in the steps above, you will need to run `renv::restore()` if this is your first time using the project.

### Tests

UI tests have been created using shinytest2 that test the app loads. More should be added over time as extra features are added.

GitHub Actions provide CI by running the automated tests and checks for code styling. The yaml files for these workflows can be found in the .github/workflows folder.

The function run_tests_locally() is created in the Rprofile script and is available in the RStudio console at all times to run both the unit and ui tests.

### Deployment

- The app is deployed to the department's shinyapps.io subscription using GitHub actions. The yaml file for this can be found in the .github/workflows folder.

### Navigation

In general all .r files will have a usable outline, so make use of that for navigation if in RStudio: `Ctrl-Shift-O`.

### Code styling 

The function tidy_code() is created in the Rprofile script and therefore is always available in the RStudio console to tidy code according to tidyverse styling using the styler package. This function also helps to test the running of the code and for basic syntax errors such as missing commas and brackets.


---

## How to contribute

Details on how to contribute to the app should go here, e.g.

### Flagging issues

If you spot any issues with the application, please flag it in the "Issues" tab of this repository, and label as a bug.

### Merging pull requests

Only members of the UfS or the Statistics Development team can merge pull requests. Add lauraselby, cjrace and sarahmwong as requested reviewers, and the team will review before merging.

---

## Contact

Add contact details of how to get in touch with your team.
