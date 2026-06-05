Title
Student Academic Advisor Expert System

Intro
This report explains the reasoning and inferencing process used in the Student Academic Advisor Expert System. The system was developed to assist universities in evaluating student academic status based on predefined rules and facts.The expert system uses a rule-based approach to determine whether a student qualifies for scholarships, graduation, academic probation, registration approval or Dean's List recognition.The system demonstrates the use of knowledge representation, forward chaining inference, and explanation facilities in a Knowledge-Based System.

Knowledge Representation
Facts
GPA
Attendance Percentage
Disciplinary Status
Completion of Prerequisite Courses
Outstanding Fees Status

Rules
Scholarship Rule
IF GPA > 3.5
AND Attendance > 80%
AND No Disciplinary Cases
THEN Eligible for Scholarship

Graduation Rule
IF GPA > 3.0
AND Completed Prerequisites
AND No Outstanding Fees
THEN Eligible for Graduation

Probation Rule
IF GPA < 3.0
THEN Academic Probation
Registration Rule
IF Outstanding Fees
THEN Registration Blocked

Dean's List Rule
IF GPA > 3.5
AND Attendance > 80%
THEN Dean's List Candidate

The system uses Forward Chaining as its primary reasoning technique.Forward chaining is a data-driven inference method that begins with known facts supplied by the user.The inference engine evaluates all rules in the knowledge base and activates any rule whose conditions are satisfied.Whenever a rule is triggered, its conclusion is added to the list of results.This process continues until all applicable rules have been evaluated.The system can generate multiple conclusions from a single set of facts.

Inference Process
Student information is entered.
Facts are stored in the knowledge base.
The inference engine evaluates each rule.
Matching rules are activated.
Conclusions are generated.
The explanation facility provides reasons for each conclusion.

Test Case 1
GPA = 2.9
Attendance = 78<img width="1600" height="1454" alt="fufhchgugiu" src="https://github.com/user-attachments/assets/495fd82e-88a0-4a70-80b6-a6e864a78e64" />
<img width="298" height="168" alt="Screenshot 2026-06-05 160003" src="https://github.com/user-attachments/assets/6713189f-17c8-4b90-88ae-ca7e0c739e4a" />
<img width="362" height="469" alt="Screenshot 2026-06-05 155901" src="https://github.com/user-attachments/assets/4325bf63-5d10-499a-bcb3-35e513aa157b" />
<img width="292" height="181" alt="Screenshot 2026-06-05 155756" src="https://github.com/user-attachments/assets/e50a0430-53f5-4f80-a964-cc1643c1a278" />
<img width="292" height="181" alt="Screenshot 2026-06-05 155756" src="https://github.com/user-attachments/assets/40d64d3a-4d8f-44ab-96f8-d24ba4fbcfc3" />
%
Disciplinary Cases = No
Completed Prerequisites = No
Outstanding Fees = No
Rules Activated
Probation Rule
Conclusion
Academic Probation
Explanation
The student was placed on Academic Probation because the GPA was below 3.0. The Probation Rule was therefore activated.

Test Case 2
GPA = 3.6
Attendance = 94%
Disciplinary Cases = No
Completed Prerequisites = Yes
Outstanding Fees = No
Rules Activated
Scholarship Rule
Graduation Rule
Dean's List Rule
Conclusions
Eligible for Scholarship
Eligible for Graduation
Dean's List Candidate
Explanation
Eligible for Scholarship because:
GPA > 3.5
Attendance > 80%
No Disciplinary Cases
Eligible for Graduation because:
GPA > 3.0
Completed Prerequisites
No Outstanding Fees
Dean's List Candidate because:
GPA > 3.5
Attendance > 80%
All conditions required by these rules were satisfied, therefore all three rules were activated.

Test Case 3
GPA = 3.1
Attendance = 87%
Disciplinary Cases = No
Completed Prerequisites = Yes
Outstanding Fees = Yes
Rule Activated
Registration Rule
Conclusion
Registration Blocked
Explanation
The student has outstanding fees. According to the Registration Rule, students with outstanding fees cannot complete registration. Therefore, registration was blocked.

Explanation Facility
The explanation facility provides transparency in decision-making by showing why a conclusion was reached.
For every conclusion generated, the system stores the facts and conditions responsible for activating the rule.
This allows users to understand the reasoning process rather than simply receiving a final answer.
Example:
Eligible for Scholarship because:
GPA > 3.5
Attendance > 80%
No Disciplinary Cases
Therefore, the Scholarship Rule was activated.

Advantages 
Provides consistent academic recommendations.
Reduces manual decision-making.
Supports multiple conclusions.
Easy to update and maintain.
Improves transparency through explanations.

Limitations
Decisions are limited to predefined rules.
The system cannot learn from experience.
New situations require additional rules.

Conclusion
The Student Academic Advisor Expert System successfully demonstrates the principles of knowledge representation, reasoning, and inferencing in expert systems. Through the use of forward chaining, the system evaluates student information and generates appropriate academic recommendations. The explanation facility enhances transparency by clearly showing the reasons behind each conclusion. This project demonstrates how Knowledge-Based Systems can support academic decision-making processes in educational institutions.
