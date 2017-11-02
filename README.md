### Table of contents
[Online discussion area](#online-discussion-area)  
[Location](#location)  
[Supplies](#supplies)  
[Projects](#projects)  
[Class topics](#class-topics)  
[Syllabus](#syllabus)  
[License](#license)  

## Viewing these materials
The class materials are best viewed at [https://mlhale.github.io/CYBR3600/](https://mlhale.github.io/CYBR3600/)

## Online Discussion Area
I have setup an online discussion board on slack.com for usage in this class. If you decide to work on a group project, I can create some private channels for you to work on, but I want to be able to participate in your conversations - so please use the space on slack.

Go to [drhale3600.slack.com](https://drhale3600.slack.com) and use your unomaha email address to register an account. Alternatively, you can use [this link](https://join.slack.com/t/drhale3600/signup).This will give you access to the class slack channel. The chat channel is for general discussions with me or your fellow classmates. The questions channel is for you to ask public questions that I will answer for the whole class. This is better than email if you think that the answer to your question might benefit everyone. You can also send me private messages. Generally I am faster at replying on slack than I am by email.

## Location
All classroom activities will take place in PKI room 252 unless otherwise noted ahead of time.

### Texts
* Information Security Governance by Krag Brotby (ISBN: 978-0470131183)
  * Book is available free online via the [Library](http://onlinelibrary.wiley.com.leo.lib.unomaha.edu/book/10.1002/9780470476017)
* [NIST SP 800-53](https://nvd.nist.gov/800-53)
* [NIST SP 800-37](http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-37r1.pdf)
* [FIPS 199](http://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.199.pdf)
* [NIST SP 800-66](http://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-66r1.pdf)
* Other Handouts TBA



## Tentative Class Topics and course overview
* Introduction and Governance ([Lecture 1 Slides](./slides/lecture1.pdf))
  * Icebreaker
  * Information Security Governance
  * Intro to Risk Management

* Risk and Strategic Decision making ([Lecture 2 Slides](./slides/lecture2.pdf), [Lecture 3 Slides](./slides/lecture3.pdf))
  * Asset Identification
  * Strategic value
  * Threats and scopes
  * Quantifying Loss
  * [**Homework: Risk and Loss**](./homework/iasc3600-homework1.pdf)
  * [Quiz 1: Risk and Governance](https://unomaha.az1.qualtrics.com/jfe/form/SV_dd0nvHadau27UeF)
  * Decision Trees
  * Risk attitude and utility theory
  * Risk Prioritization
  * [Example Decision Tree problem](./slides/example-decision-tree-problem.md)
  * [**Homework: Decision Trees**](./homework/iasc3600-homework2.pdf)
  * [Extra practice problems](./slides/extra-practice-atle-decision-trees.md)
  * [Quiz 2: Probabilistic Risk and Decision Trees](https://unomaha.az1.qualtrics.com/jfe/form/SV_9B260NG5oRPNxqZ)

* High Level Policy Creation ([Lecture 4 Slides](./slides/lecture4.pdf))
  * Business and governance requirement gathering
  * Scopes and functions of different policy documents
  * Internal consistency and style
  * Defining Roles and Responsibilities
  * Policy metrics and measurements
  * [Homework: Policy review and Analysis](./homework/projects/project-1.md)

* U.S. Compliance Laws and Security Controls ([Lecture 5 Part 1 Slides](./slides/lecture5-1.pdf), [Lecture 5 Part 2 Slides](./slides/lecture5-2.pdf))
  * Policy concerns by security domain
  * Aligning Policy with regulations and standards
  * Overview of HIPAA, GLBA, SOX, FERPA
  * Focus on [FISMA](http://csrc.nist.gov/drivers/documents/FISMA-final.pdf)
  * Security Control standards
    * [FIPS 199](http://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.199.pdf)  
    * [FIPS 200](http://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.200.pdf)
    * [NIST SP 800-37 ](https://csrc.nist.gov/publications/detail/sp/800-37/rev-1/final)
    * [NIST SP 800-53 ](https://csrc.nist.gov/publications/detail/sp/800-53/rev-4/final)
    * [National Vulnerability Database resources](https://nvd.nist.gov/other)
  * [NIST SP 800-66](http://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-66r1.pdf)
  * [Quiz 3](https://unomaha.az1.qualtrics.com/jfe/form/SV_0oz0NLR5xXr7ZjL)
  * PCI DSS
  * COBIT 5
  * ISO 27002
  * Common Criteria
  * Maturity Model

* [**Project: Business Creation and Product FISMA Certification**](./homework/projects/project2.md)
  * Assess business security program maturity
  * Identify business assets
  * Select Security Controls
  * Assess information systems against selected controls

* Formal methods for policy representation and certification ([Lecture 7 Slides](./slides/lecture7.pdf)
  * Propositional and First-order logic
  * Representing policies in first-order logic
  * Stating non-compliance formally
  * [In-class Logic Exercises](./slides/in-class-logic-exercises.md)
  * [**Homework: Formal Logic**](./homework/logic-homework.md)
  * State-based temporal models
  * Covert channels
  * Access Control Matrix

* **Certification Project Presentations**

* Information Flow Control & Policy Composition ([Lecture 8 Slides](./slides/lecture8.pdf), [Lecture 9 Slides](./slides/lecture9.pdf))
  * Multi-domain policies
  * Dealing with third parties
  * Composable informal and formal policies
  * Detecting policy constraint violations

* Security Awareness and Training
  * Constructing an enterprise-wide training plan
  * Protecting against social engineering
  * Protecting against “Post-it note” style problems
  * **Project: Security Awareness and training plan**

* **Final Exam**


## Syllabus
**Date/Time**: Tuesday/Thursday 1:30pm – 2:45pm  
**Instructor**:  Dr. Hale  
**Office**:  PKI 174-D, `(402) 554-3978`  
**Office Hours**:  Open door policy, or by appointment  
**E-mail**:  `mlhale@unomaha.edu`  


### Course Abstract
Policy is an integral element of Information Security within and across organizations. This course will cover the development of security policies and procedures at an organizational level, how such policies are intertwined with regulatory compliance necessities, and the legal, ethical, and financial implications of policy. Students will leave with the ability to go into an organization and understand the basis for and effect of IT policies. Students will also be able to apply policies to information systems and cover human factors such as constructing a security awareness campaigns to satisfy operational security controls and prevent attacks such as phishing and spear phishing.


### Grading Breakdown (due dates are tentative)
 * (10%) Class participation
 * (40%) Homework & Projects
 * (20%) Quizzes
 * (30%) Final Exam

Each project will have a specific grading rubric that includes the core requirements for the project (i.e. what the application must do), any required intermediate milestone goals (such as short progress meetings with the instructor), the project due date, and the list of items that must be submitted. At least one of the projects will include a presentation component to be presented in class on the project due date.  

### Attendance
* Class Attendance: Attendance is highly recommended, there are a number of in-class participation measures, so if you miss class your grade may suffer.
* Presentation Attendance (Mandatory): If you miss class on a presentation day (Dates TBA) you will receive a 0 on the presentation portion of the project grade unless you have a university-approved excuse or an approved extension (see below).

### Group Work
Students may choose (or be compelled) to work in groups on certain assignments. Group work may optionally (at the discretion of the instructor) include an individual participation grade worth 40% of the total group points, e.g. a group may make a 100% on a particular project, but an individual with low participation in the group may make a 60%.

### Team formation
The instructor reserves the right to make a change to any team or any project during the course of the semester for any reason that may or may not be disclosed. Project rescoping will be performed in this event.

### Service Learning / Real World Customers
As part of UNO’s strategic initiatives, individuals or groups may be partnered with community organizations in Omaha for service learning. If community partners can be identified, student projects (group or individual) in the class may be directed at meeting community needs. In the event of community projects, appropriate scoping will be considered to ensure that community needs can be met within the time constraints of the coursework.

### Project Extensions and Late work
Sometimes unforeseen events occur or work takes longer than expected. In such cases, an extension may be requested. To receive an extension, individuals or groups must request an extension at least 24hours in advance of the due date. Extension time frames are at the discretion of the instructor, but generally will not be longer than 1 week. Failure to request an extension 24 hours prior to the due date means that the work is due at the specified time. Granting extensions is at the discretion of the insturctor. Late work without a requested extension will receive a 5% point reduction per day up to a total of 40%. Late work submitted 8 days after an original (or extended) due date will not be accepted.

### Special accommodations for students with disabilities
Students with disabilities requiring special accommodations must contact disability services. Disability services may be reached by phone at (402) 554-2872 or by email at unodisability@unomaha.edu.

### Special accommodations for active duty or reserve military
Students serving in the military requiring special accommodations (e.g. unit deployment) must contact the office of Military and Veteran Services by phone at (402) 554-2349 or by email at unovets@unomaha.edu.

### Plagiarism
The university policies on cheating and plagiarism apply in this course. Except on designated group work, the expectation is that every student will do their own work. Students under suspicion of plagiarism for individual assignment submitted materials will be given an opportunity to defend themselves. If after defense the instructor still believes the work to be plagiarized the department chair will be notified and the grade evaluation for the assignment will be lowered to a value between 50% and 0% at the discretion of the instructor. If a second occurrence of plagiarism occurs, the student will receive an F for the course and the registrar’s office will be notified that the student is not permitted to withdraw from the course. In addition the department chair and dean will be notified.

### Work Retainment
The CS and IS programs in the College of IS&T are accredited through ABET (the Accreditation Board for Engineering and Technology. This organization occasionally requires that we keep samples of student work.

The instructor may retain a copy of your exams (with names and any other identifying information removed) for accreditation or pedagogy purposes, unless you specify otherwise in writing.

In addition, the instructor retains the right to use any code or project artifacts developed in the course for pedagogy, research, or service learning purposes. Student web project code developed in the course may be used in future secure project development courses, by the instructor for research purposes, or by designated stakeholders.

## License  
Information Security Policy
Copyright (C) 2017  Dr. Matthew L. Hale

### Lesson content
Copyright (C) [Dr. Matthew Hale](http://faculty.ist.unomaha.edu/mhale/) 2017.  

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">This lesson</span> is licensed by the author under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.

### Software affiliated with the course
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.

#### What does GPLv3 mean?
[tl;drLegal summary](https://tldrlegal.com/license/gnu-general-public-license-v3-%28gpl-3%29)
