### Feedback given to LLMs (ChatGPT and Llama) as prompts
The following text is an example of how feedback was given to the LLM.

USER: Hi, I have a task for you. I am currently conducting research on Detecting and Resolving Ambiguities in User Stories with the help of LLMs. Can you help me answer a series of questions for my research? 

**LLM: Of course! I'd be happy to help you with your research on detecting and resolving ambiguities in user stories. Please feel free to ask your questions, and I'll do my best to provide thorough and helpful responses.**

USER: When you are asked a question: "Is the provided user story ambiguous? If the user story is ambiguous, resolve the ambiguity by rewriting the user story with the help of QUS framework." follow the following rules:

_-- Here QUS framework was provided to the LLM same as in Table I --_

Following are the two types of responses expected:

1. Response type for ambiguous user stories: 

Answer: Yes, the user story is ambiguous..  The resolved user story is: _[rewrite the new version of user story by removing the ambiguity]_.

2. Response type for unambiguous user stories: 

Answer: No, the user story is not ambiguous because _[specify reasoning here]_.

Following are the examples to help you understand the nature of questions and answers. Please remember each example for future questions.

**LLM: Got it! Please provide the examples, and I'll keep them in mind for future questions.**

USER: Example 1:

Question: User Story: “As an admin of the system, I want to add or delete recycling center information in the system database, so that I can keep the database up-to-date over time.” Is the provided user story ambiguous? If the user story is ambiguous, resolve the ambiguity by rewriting the user story.

Answer: Yes, the user story is ambiguous. A user story must always be atomic, which means only one feature is present in the user story. The solution to fix this ambiguity is by dividing the user story into two different user stories.

Solution: User story 1: As an admin of the system, I want to add recycling center information in the system database so that I can have a list of all recycling centers.

User story 2: As an admin of the system, I want to be able to delete recycling center information in the system database so that the old data is not there.

_-- Similarly to Example 1, three more examples were provided to the LLM --_


**LLM: Got it, I'll keep the examples in mind. Please go ahead and ask your questions, and I'll provide responses based on the provided examples.**

USER: Question: User Story: “As a user of the system, I want to get feedback when I enter an invalid zip code.” Is the provided user story ambiguous? If the user story is ambiguous, resolve the ambiguity by rewriting the user story with the help.

**LLM: No, the provided user story is not ambiguous because it follows the standard user story template and expresses a clear feature and rationale.**

USER: The user story is ambiguous since it does not specify the feature correctly

**LLM: You're correct. I apologize for the oversight. The user story is ambiguous because it lacks clarity on what kind of feedback the user expects upon entering an invalid zip code. Let's resolve the ambiguity:**

**Solution: "As a user of the system, I want to receive a clear error message when I enter an invalid zip code, so that I can correct it and proceed with my task."** 
