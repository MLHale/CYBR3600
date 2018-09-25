# CYBR3600 Homework 4 (Project 2): NIST / FISMA Compliance Project
Due Date: Thursday 10/11/18 by Class time (1:30PM)  
Class Lab Time: Thurs. 9/27/18, Tues. 10/2/18
Presentations 10/11 and 10/16

## Overview
In this project you will pick a company, identify its strategic goals and maturity, and then step through the FISMA/NIST certification process to examine a system for new acquisition. You will receive (lab) time in-class to work on your project and ask any questions you may have.

As part of this assignment, you will *first pick a company* and then *prepare a document* with the following structure:

1. Strategic company information
2. Company Maturity
3. System information
4. System Assessment & Certification Recommendations

Each section is discussed in detail below.

### Strategic Company information
#### Task
The purpose of this part of the assignment is to identify important strategic information that guides how the company operates.

#### Report Structure
The `Strategic company information` section should contain the following:

1. `Name` - The company's name
2. `Executive Summary` - Write an executive-summary (max three paragraphs) synopsis of what your company does. When writing your summary answer questions such as, what products and services the business offers, what its customer base is, how maturity is the organization (e.g. is it a startup or an established company?), what risks does it face, how does it make money?
3. `Strategic Business Goals` - In a bulleted list under the summary, identify at least 5 business goals/objectives associated with the company, (i.e. what are they trying to achieve as a business?). Include a sentence for each that explains the goal. **DO NOT** list `make money` or `grow` as business objectives. Be specific. For instance, a goal for `Google` might be `Improve search precision` or `Increase ad product targeting through embedded in-home IoT products`
4. `IT Function` - Below that write a single paragraph about how IT supports your company to achieve its stated goals.

### Company Maturity
#### Task
The purpose of this part of the assignment is to identify how mature your company is with respect to its information security and IT processes. Look to existing company policies and make your best guesses about the company, as you do the following:

Open the attached [ISO/NIST maturity assessment tool](https://github.com/MLHale/CYBR3600/raw/master/homework/projects/assessment-tool.xlsm) and identify the company’s maturity levels. The tool has a number of questions you can ask yourself about the company. For each question, assign your answer a value of `Not performing (0)` to `continuously improving (5)` or `Not applicable`. Your selections should fit with the governance objectives and business goals of your company. For instance, if you are a startup you probably don’t have 5s across the board in info. Sec. You will be graded by how well your protection profile maps to your company goals. Attach your spreadsheet to your submission.

#### Report Structure
The `Company Maturity` section of your report should just contain a single sentence that identifies how mature your company is and reports your overall maturity value calculated from the assessment tool spreadsheet.

### System Information
#### Task
Assume your company is looking to acquire and use a new system. Pick an off-the-shelf piece of software of your choice for the company to acquire. Identify how the company might use it, the assets that might be involved in its use, and then identify the criticality of the system.
> Selecting a mature open source product with a large community is wise - because it means there will be more information available about it.

#### Report Structure
The `System Information` section of your report should contain the following:

1. `Name of Product` - The name of the software you are examining and a link to where the software documentation (e.g. Github repository).
2. `Usefulness` - Identify how your selected company might use this software.
3. `Related Assets` - Identify relevant company assets that this software might interact with (E.g. will it use PII, intellectual property, etc). Be specific - don't list 'information'. Example: my product might be a point-of-sale system like [Shopkeep](https://www.shopkeep.com/) and I might be looking at a retail chain. In this case, assets might be customer data such as name, address, credit card data, etc.
4. `Criticality Assessment` - Use FIPS 199/200 to identify a criticality for the system based on your strategic objectives above and the use the company might have for the system, and the importance of the related assets. You should list the FIPS-specified tuple for each aspect of criticality.

### System Assessment
#### Task
Given your previous work and the criticality assessment, select a NIST SP800-53 security control baseline appropriate for your system using the 800-53 Low/Moderate/High baselines. Once selected, pick a subset of controls from the baseline and assess your selected system against them. Your report must state which controls you are assessing, how you assessed them, and should provide evidence that supports your claims.

#### Report Structure
The `System Assessment & Certification Recommendations` section should be structured as follows.

1. `Assessment Summary` - Given your assessments, sum up the overall results and state whether or not the system would be appropriate to use for the company for the identified purpose. Is it secure? Does it meet strategic goals? Does it protect assets? Are there issues off-the-shelf?
2. `Specific results` - This section should be a table structured using the exact headers listed below. If it doesn't fit neatly into your report document, you may attach an .xls, .xlsx, or .csv file with the table.

Your table should be structured as follows. Use these exact headers.

| Control in baseline | Compliant	| Confidence | Control Text	| Method of Assessment | Compliance Evidence | Mitigation Suggestions |
|---------------------|-----------|------------|--------------|--------------|--------------------|--|
| The control identifier | Yes/No/Partially | Scale 1 (not confident) to 5 (confident) based on how confident you are in your compliance assessment | The actual control text for the control identifier | The specific process you followed to measure/gauge compliance. Considering using checklists from NVD (https://nvd.nist.gov/ncp/repository) if applicable. | The specific evidence you found by conducting the method of assessment that supports your claim | Discuss the mitigations that should occur to make the system compliant with this control, given your compliance findings|

*Example:*

| Control in baseline | Compliant	| Confidence | Control Text	| Method of Assessment | Compliance Evidence |
|---------------------|-----------|------------|--------------|--------------|--------------------|
AU-2.a | No | 5 | The organization Determines that the information system is capable of auditing the following events: [Assignment: organization-defined auditable events] |I examined the software documentation and source code to identify audit functionality in the app. |	There was no audit component present, so the system is by default not able to capture the events.|
SC-8(3) |	Yes| 3 |The information system implements cryptographic mechanisms to protect message externals unless otherwise protected by [Assignment: organization-defined alternative physical safeguards].	| I checked the app to see if it uses TLS/SSL and to ensure other system users could not view traffic that was not their own. |	The webservice uses TLS/SSL (https). Personnel messages are protected by the functionality in messenger.php and the audit system (code files in /var/www/html/audit). I could only access headers and routing information for messages sent to me, messages sent by me to target users, or if I was using a system admin account.

## Submission
Prepare a report, of type .md, .pdf, .doc, .docx only, that contains the listed sections above in the format specified. Submit your report to Canvas by the due date.

## Presentation
You will also prepare and present the findings of your project in a brief 5 min presentation. To keep things moving, you should structure your presentation around answering the following questions:

1. What company did you choose?
  * Briefly address: What does your company do, i.e. what are their strategic objectives and goals?
  * Briefly address: How mature is the company in terms of information security? What resources (generally speaking) did you use to determine this maturity?
2. What system did you choose? 
  * Briefly answer, what does it do? I.e. what functions/services does it offer?
  * How was your system categorized according to FIPS 199/200?
  * Which Security control baseline did you pick for the system?
3. What did you assess?
  * Which specific controls did you pick from the baseline?
  * How did you assess them against the system you choose?
  * What were your findings? Was the system compliant or non compliant with the controls?
  
### Presentation Grading Criteria
Your presentation will be graded using the following Rubric

| | Meets expectations (9-10) | Some Issues (6-8) | Does not meet expectations (0-5)|
|---|---|---|---|
| Enthusiasm and clarity | Presenter exhibits enthusiasm about the work and speaks clearly and confidently. | Some issues with clarity and enthusiasm. | Presenter has mumbles, is not clear, and/or does not demonstrate any enthusism. |
| Understanding | Presenter understands all aspects presented about the project. | Some gaps in understanding when questioned by audience or routinely looks at team slides |Poor understanding of project. |
| Relevant information | Engaging relevant information is presented about the project. | Valuable information is presented but there are multiple tangents. | Little valuable information is presented |
| Quick overview of Company | Overall company information is succinct and informative. | Too much time is spent on company details or important details are lacking. | Way too much time is spent on company info or details are not covered at all. |
| Overview of System details| System for assessment is adequately described. | Some details regarding the system are missing or unclear or far too much time is spent on discussing the system. | Way to much time spent or no coverage at all. |
| Assessment | Control assessments procedures pursued are clearly defined and discussed. | Assessment information is insufficient. | Few or no details of assessment are discussed. |
| Results / Findings | The findings of assessment are clearly discussed. Results identify whether or not the system or product are compliant with the security controls and any other relevant outcomes. | Results are missing or unsupported by the work conducted. | Few or no results are presented. |
