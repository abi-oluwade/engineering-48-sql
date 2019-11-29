Sparta Day 8

# Joins and Subqueries

- Understand the Various JOIN types available within SQL
- Determine the differences between JOIN types using SET theory.
- Discover the power of a subquery.

## Today we’ll be doing advanced SQL, more specifically utilising the JOIN keyword and all the variations of it such as INNER JOIN.
For join:
-	Figure out what info we need
-	Join the tables joining them where the columns share related data.
Joins
A JOIN clause is used to combine rows from two or more tables, based on a related column between them.
1.	INNER JOIN (simple join)
The most frequently used variation of join, it returns any rows where they is a matched key in BOTH tables. So below is an example of the general synthax when producing a JOIN.
SELECT <columns>
FROM <left_table>
INNER JOIN <table_name)
ON <left_table_column_key> = <right_table_column_key>
2.	RIGHT JOIN
Return all the rows from the right table, and the matched rows from the left table regardless of any matched rows in the left.
3.	LEFT JOIN
The LEFT JOIN keyword returns all records from the left table (table1), and the matched records from the right table (table2). The result is NULL from the right side, if there is no match.
4.	FULL JOIN
The FULL OUTER JOIN keyword returns all records when there is a match in left (table1) or right (table2) table records.
-  Aliasing can be useful when dealing with multiple tables and can be done simply by placing a space after the <table_name> so for example ‘FROM student s’ will alias the student table name to just ‘s’
- We can also use the ‘FORMAT’ keyword to display different ways of displaying the data.

# Subquery
-	The most common place to use a subquery in within WHERE but can also be used in place of a JOIN keyword.
-	Subqueries are ALWAYS in parenthesis.

# Agile
There is no single variant of agile, the value & principles ARE important.
Agile arose due to the common methodology used before where there was too much upfront analysis, restricted change control and too much uncertainty.
They took down a set of underlying values and principles:
“We are uncovering better ways of developing software by doing it and helping others do it. Through this work we have come to value”
	 - Individual and interactions (over processes and tools)
	 - Working software (over comprehensive documentation)
	 - Customer collaboration (over contract negotiation)
	 - Responding to change (over following a plan)

# “The AGILE manifesto”
Without Agile: Poor customer feedback and inconsistent planning as it is hard to plan long-term due to uncertainty. Set up change control processes to make it harder for customers to change their mind.
With Agile: Came together to discuss what was working and wasn’t. Focus on the values/principles NOT JUST THE PRACTISES.
  - As new events unfold, the project team incorporates those into realities into the ongoing work.
  - Change become opportunities to add value instead of being obstacles to avoid.

# SCRUM
Scrum is a team-based framework to develop complex systems and products. (which is the implementation of AGILE for teams)







## Scrum Framework and Roles

 - A scrum sprint is a regular, repeatable work cycle in scrum methodology during which work is completed and made ready for review. Scrum sprints are basic units of development in the scrum methodology.
The sprint backlog is a list of tasks identified by the Scrum team to be completed during the Scrum sprint. During the sprint planning meeting, the team selects some number of product backlog items, usually in the form of user stories, and identifies the tasks necessary to complete each user story.

- Sprint planning is a collaborative effort involving a ScrumMaster, who facilitates the meeting, a Product Owner, who clarifies the details of the product backlog items and their respective acceptance criteria, and the Entire Agile Team, who define the work and effort necessary to meet their sprint commitment.

- The sprint retrospective is a meeting facilitated by the Scrum Master at which the team discusses the just-concluded sprint and determines what could be change that might make the next sprint more productive. It often also helps management to get feedback from the team about the work and progress of project.
  -	Identify what went well and what needs improvement.
  -	Create a plan for improvements.
  -	Timeboxed to 3 hours for a month-long Sprint or less if shorter sprint.

- The sprint review is performed by someone externally, and overall the framework is lightweight and simple to understand; however, it is hard to master as you can get deviated. The sprint review is an informal meeting which the development team, the scrum master, the product owner and the stakeholders will attend. The team gives a demo on the product and will determine what are finished and what aren't.
  -	Informal discussion about what was done during the sprint and to adapt the product backlog.
  -	Explain what has been don’t and what hasn’t and agree on the definition of done.
  -	Demonstrate the working package.
  -	Review timeline, budget and capabilities.
  -	Timeboxed to 4 hours for a month-long Sprint or less if shorter Sprint.

## The 3 pillars of scrum:
Adaptation, Inspection and Transparency.
1.	Everyone presents the facts as is & collectively collaborates for the common organizational objective. No one has a hidden agenda. (*Transparency*)
2.	Not done by an inspector but by everyone on the Scrum Team. The inspection can be done for the product, processes, people aspects and practises. *(Inspection*)
3.	Is about continuous improvement, to adapt based on the results of the inspection. Everyone should reflect on how to improve. (*Adaptation*)

## ROLES & ACCOUNTABILITY (SCRUM TEAMS)
-	Engaged with the customers
-	Self-Organising
-	Cross functional
-	Co located

Product Owner:
  -	Key stakeholder who should have deep understanding of the product and communicated with both the team and other stakeholders.
Scrum Master:
  -	Ensures the team keeps to the values of Scrum, facilitates meetings and removes impediments/ problems from the team.
Scrum Team
  -	3-9 people
  -	All doing whatever they need to ensure the tasks is completed.
  -	Everyone is not just committed, they are involved.

## Retrospectives
-	The purpose and benefits of retrospectives

The retrospectives are present after the sprint review.
What went well- What could be improved-Actions

## Root Cause Analysis
You ask questions to get to the root of the issue, such as testing.
User Stories, Backlog and Estimation
  - Features, Epics and user stories
  - User personas
  - Acceptance criteria
  - How to write a user story

## User Stories
User stories do not include all the detail - they are only a pointer to the real requirement.
“As a <type of user>, I want <goal> so that <reason>.”
There are 2 primary ways to add more detail:
  1.	Splitting
  2.	Conditions of Satisfaction/Acceptance criteria.
- When writing good user stories:
  1.	Understandable
  2.	Follow As a … I want … So that
  3.	Independent
  4.	Negotiable
  5.	Valuable
  6.	Estimable
  7.	Small
  8.	Testable

## ESTIMATION AND PRIORTISATION BACKLOG
Product backlog – Agile teams estimate effort in various forms. It can represent time or “story points”; an abstract measure of effort needed to complete this requirement.

## Planning Poker
-	Decide on a scale, for example 1to 5.
-	Issue planning poker cards to each team member, each card has a single number on it 1 to 5.
-	The team discusses the effort of completing a task before revealing cards at the same time
-	If there is a big difference in values revealed, the team discusses the reason behind the smallest and largest values then has another round until consensus is reached.

## Business Value
Backlog Refinement
-	Removing user stories that aren’t relevant.
-	Creating new user stories as a response to needs
-	Re-assessing priority
-	Assigning estimates
-	Correcting estimates
-	Split stories that are high priority but too large to fit in an upcoming iteration.
Definition of Done (D.O.D)
