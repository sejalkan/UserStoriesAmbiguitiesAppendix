## Prompts used for Cognitive Verifier technique

#### When you are given a user story and asked a question to detect and resolve ambiguities in the user story follow these rules for a better response:
1. Check if user story is free of syntactic ambiguity:
   
      1.1. Atomic-  a user story does not follow a composite structure and expresses only one requirement for exactly one feature of the system. More than one feature can be broken down into different user stories.

      1.2. Minimal- a user story contains nothing more than a role, means, and end.

      1.3. Well-formed- a user story must always look like: “As a user _[specify role]_ I want to [specify means9 so that _[specify end]_”.

2. Check if user story is free of semantic ambiguity:

      2.1. Conflict-free-  a user story should not be inconsistent with any other user story.

      2.2. Conceptually sounds- the means express a feature and the ends expresses a rationale, not something else.

      2.3. Problem-oriented- a user story only specifies the problem, not the solution to it.

      2.4. Unambiguous- a user story avoids terms or abstractions that may lead to multiple interpretations.

3. Check if user story is free of pragmatic ambiguity:

      3.1. Complete- no steps are missing to implement the user story.

      3.2. Independent- the user story is self-contained, avoiding inherit dependencies on other user stories.

      3.3. Scalable- user stories do not denote too coarse-grained requirements that are difficult to plan and prioritize.

      3.4. Uniform- all user stories follow the template: “As a user _[specify role>]_ I want to _[specify means]_ so that _[specify end]_”.

      3.5. Unique - every user story is unique, duplicates are avoided.

4. If no ambiguity is detected the user story is not ambiguous.

5. Lastly, mention the type of ambiguity detected either syntactic, semantic, pragmatic or unambiguous.

#### After checking all the rules, following are the two types of responses expected, choose the one appropriate:

1. Response type for ambiguous user stories:

**Answer:** Yes, the user story is ambiguous as it mentions [specify reasoning here]. 

The detected ambiguity is _[specify type of ambiguity here]_ in.

The resolved user story is: _[specify new version of user story by removing the ambiguity]_.

2. Response type for unambiguous user stories:

**Answer:** No, the user story is not ambiguous because _[specify reasoning here]_.

**Prompt input:**

**Question:** According to the rules to detect and resolve ambiguities, check if the provided user story is ambiguous. If it is ambiguous, mention the type of ambiguity that exists and a resolved version of the user story by removing the ambiguity. If it is unambiguous, specify that.

**User story:** As a user of the system, I want to be able to check the history of waste I recycled as well as keep a record of it,  so that I can review previous waste deposits.
