# Extra practice problem
You are a security analyst that is consulting with Fictional Medical Center (FMC). FMC is required by law to be HIPAA compliant. 

The federal government provides the following data regarding HIPAA Violations:

| Violation Class | Fine for each Record Violated | Max cost per year |
| --------------- | ----------------------------- | ----------------- |
| Class A – Did not know | $100-$50,000 | $1,500,000 |
| Class B – Reasonable Cause | $1,000-$50,000 | $1,500,000| 
| Class C (i) – Willful Neglect (corrected) | $10,000 – $50,000 |  $2,500,000| 
| Class C (ii) – Willful Neglect (not corrected) | $50,000 | $5,500,000 |

FMC provides the following information about their hospital.  
_Our patient data consoles (the ones that nurses and techs use in hospital rooms) report daily statistics to a central hospital-wide server that stores the data in a large MySQL database. Below is a summary table that shows how often different threats have affected these consoles and the type of HIPAA violation each causes._

| vulnerability | Incident frequency | Avg. Number of Patient Records Affected | HIPAA Violation Class |
| ------------- | ------------------ | --------------------------------------- | --------------------- |
| Connecting to Wifi-Pineapple/Rogue Access Point | 10/Month | 5 | Class A |
| Insecure message handling | 1 every 8 Months | 125 | Class C |

FMC also states the following:
* _50% of our Class A violations cost us $500, 25% cost $1,000, and 25% cost $10,000_
* _We’ve not had any Class B violations_
* _20% of our Class C violations incurred the maximum fine. The other 80% incurred the minimum._
* _We have not had any Class C(ii) violations, since we always attempt to correct cases of willful neglect._

a) State the two security threats quantitatively using Expected Threat Impact (ETI) and Annual Threat Loss Expectancy (ATLE). Show your work. 

b)	Given your calculations in a) you confer with the vendor of the data consoles to resolve the security vulnerabilities. They tell you that they can implement a Rogue AP detection kit and that it should cost 1.5 Million dollars to develop and deploy to all of the consoles that FHC has. They claim there is a 50% chance that it will overrun its budget and cost 2 Million Dollars, since they are afraid that some consoles may need to be wiped and overwritten to accept the patch. Regarding the message handling system, they claim that they can write and deploy a separate patch for the FHC consoles for 3 Million dollars, but that there is a 50% chance it will greatly overrun its budget (because the messaging infrastructure is old) and, therefore, cost 6 Million dollars. Draw a single decision tree that describes the different options. 

c) Pick the best option for the hospital assuming they have a risk neutral attitude and they are only optimizing for year one. Show the cost for each option as computed from the tree (you can show it on your graph above, but indicate if you do so).

d) Would you make the same decision if you looked at a two year period? If not what decision would you choose?

[Click here for the solution](extra-practice-atle-decision-trees-solution.md) - Try it first!
