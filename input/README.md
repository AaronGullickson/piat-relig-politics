# Data Source Description

We are using data from the [Cooperative Election Study](https://cces.gov.harvard.edu/) (CCES) in 2020. The CCES is a 50,000+ person national representative survey of the US population that is focused on political attitudes and behavior. 

From the full data, I have extracted and recoded the following variables for our use as an analytical dataset. To load this dataset in R, you just need to run the setup code chunk in the full_report.Rmd R Markdown document. The name of the dataset in R is `cces`. 

* **conservative**: This is a 7-point scale indicating the respondent's political ideology on scale from "Very Liberal" (1) to "Very Conservative" (7), with the value of 4 representing "Middle of the road." This is the key dependent variable.
* **party_affil**: The respondent's party affiliation. Either Democrat, Republican, Independent, or Other.
* **relig**: The respondent's religious affiliation. This measure is **not* religiosity but is something you will want to consider controlling for in models.
* **gender**: The respondent's gender.
* **education**: The respondent's highest degree received. This is the key contextual variable.
* **race**: The respondent's race.
* **age**: The respondent's age.
* **family_income**: The family income of the respondent measured in 1000s of dollars. This measure was actually recorded in brackets of income (e.g. $50,000-59,999). I have taken the midpoint value of each bracket to give you an additional quantitative measure.
* **religiosity**: A scale measure of a person's religiosity. This measure is taken by combining the responses to how important religion is for the respondent, how frequently the respondent attends religious services, and how frequently the respondent prays. The scale is designed to have a mean of zero and a standard deviation of 1. High values mean high levels of religiosity and low (negative) values mean low levels of religiosity. This is the key independent variable.
