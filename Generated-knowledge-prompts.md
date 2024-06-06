## Prompts used for Generated Knowledge technique
I am currently conducting research on Detecting and Resolving Ambiguities in User Stories with the help of LLMs. Can you help me answer a series of questions for my research? 
Following are examples of types of ambiguities that may appear in user stories with explanations of why they are ambiguous. This shall help you understand how to detect and resolve ambiguities in user stories: 

1. **Input:** User story: As a User, I’m able to click a particular location from the map and thereby perform a search of landmarks associated with that latitude longitude combination
    
   **Knowledge:** The user story contains syntactic ambiguity because it is not atomic since in the user story two features which are clicking on a location and search landmarks are mentioned. An atomic user story must contain only one feature. 

2. **Input:** User story: As a care professional I want to see the registered hours of this week (split into products and activities). See: Mockup from Alice NOTE: - First create the overview screen - Then add validations

   **Knowledge:** The user story contains syntactic ambiguity because it is not minimal since in the user story mockup ideas are mentioned. A minimal user story must contain nothing more than a role, means and an end.

3. **Input:** User story: Add static pages controller to application and define static pages

   **Knowledge:** The user story contains syntactic ambiguity because it is not well-formed. A well-formed user story must contain a role and follow the template. “As a (…), I want (…), so that (…)”.

4. **Input:** User story: As a User, I want to open the interactive map, so that I can see the location of landmarks.

   **Knowledge:** The user story contains semantic ambiguity because it is not conceptually right since the part of ‘seeing location of landmarks’ in the user story refers to a need of another user story. A conceptually right user story mentions a feature and expresses a rational end without referencing other user stories.

5. **Input:** _User story A_:  As a User, I’m able to edit any landmark. _User story B_: As a User, I’m able to delete a landmark which I added

   **Knowledge:** The user stories contain semantic ambiguity because of existing conflicts within the user stories since User Story A says ‘any landmark’ but User Story B refers to landmarks that users have added.

6. **Input:** User story: As a care professional I want to save a reimbursement. - Add save button on top right (never grayed out).

   **Knowledge:** The user story contains semantic ambiguity because it is not problem-oriented and also hints at the solution which is ‘add save button on top right’. A problem-oriented user story must express the need for a feature but not the solution to do it.

7. **Input:** _User story A_: As a Visitor, I’m able to see a list of news items, so that I can stay up to date on news. _User Story B_: As a Visitor, I’m able to see a list of news items, so that I can stay up to date on news 

   **Knowledge:** The user stories contain pragmatic ambiguity because they are not unique. A unique user story is when no features are duplicated.

8. **Input:** User story: As an Administrator, I receive an email notification when a new user is registered 

   **Knowledge:** The user story contains pragmatic ambiguity because it is not uniform. A uniform user story follows the standard user story template which is: “As a (…), I want (…), so that (…)”.

9. **Input:** User story: As a care professional I want to see my route list for next/future days, so that I can prepare myself(for example I can see at what time I should start traveling)

   **Knowledge:** The user story contains pragmatic ambiguity because it is not scalable since it is unclear what ‘my route list’ implies to. A user story is scalable when it is small and specific, so that the estimation is easier. 

10. **Input:** User Story: Server configuration 

    **Knowledge:** The user story contains pragmatic ambiguity because it is not a full sentence. A user story should be a well-formed full sentence and follow the standard user story template which is: “As a (…), I want (…), so that (…)”. 

11. **Input:** _User Story A_: As an Administrator, I am able to add a new person to the database followed by. _User Story B_: As a Visitor, I am able to view a person’s profile the database.

    **Knowledge:** The user stories contain pragmatic ambiguity because they are not independent since ‘User Story B’ depends on ‘User story A’. A user story is independent when it is schedulable and implementable in any order, regardless of other user stories. 

12. **Input:** User story: As a User, I am able to edit the content that I added to a person’s profile page

    **Knowledge:** The user story contains semantic ambiguity because the word ‘content’ is ambiguous and can lead to multiple interpretations. An unambiguous user story must be clear and have only one interpretation.

13. **Input:** User Story: As an Administrator, I am able to view content that needs to be reviewed 

    **Knowledge:** The user story contains pragmatic ambiguity because it is not complete since the word ‘content’ in the user story is unclear. A complete user story creates a feature-complete sentence without missing any steps.

**Prompt:** 
**Input:** User story: As a user of the system, I want to be able to check the history of waste I recycled as well as keep a record of it,  so that I can review previous waste deposits.

**Question:** Is the provided user story ambiguous? If the user story is ambiguous, specify the ambiguity based on the QUS framework (choose either syntactic, semantic or pragmatic) and the user story template which is: following the format "As a (..), I want (..), so that (..)". If no, please write no.
