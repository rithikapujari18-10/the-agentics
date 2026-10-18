# CrewAI Assignment Report

**Name:** Rithika Pujari  
**Topic I used:** How artificial intelligence helps students learn

## 1. What I changed

I changed the Technical Writer agent's backstory in `main.py`. I instructed it to explain difficult topics to 10-year-old children using simple English, short sentences, everyday examples, and step-by-step explanations. I chose this change because I wanted to see how changing an agent's instructions affects the final explanation.

## 2. How CrewAI works

CrewAI organizes AI agents and tasks into a team called a crew. In my project, the Research Analyst gathers and organizes information about the topic. The Technical Writer uses that information to create an explanation, and the Editor reviews the result.

An agent has a role, a goal, and a backstory that guide its behavior. A task describes the work the agent must complete and the expected output. The crew coordinates the agents and their tasks to produce the final result.

Changing the Technical Writer's backstory gives it different instructions about its audience and writing style. This can change the words, examples, and level of detail used in the explanation.

## 3. Evidence

I saved the original execution log in `run1_original.txt` and its explanation in `explainer_run1.md`. After changing the Technical Writer's backstory, I ran the workflow again with the same topic and saved the results in `run2_changed.txt` and `explainer_run2.md`.

Comparing the two explanations helps show whether the new instructions resulted in simpler language and more accessible examples.

One challenge was configuring the project to use the Groq model correctly. I checked the model configuration and tested the connection before running the workflow successfully.

## 4. Choosing a framework

I would choose CrewAI for a project that requires several AI agents to perform different roles, such as researching a topic, writing an explanation, and reviewing the result. Its agent and task structure makes it easier to organize this workflow and understand each agent's responsibility.

The Agents SDK is another framework we studied. It may be a good choice when building applications around agent handoffs and tool use. Depending on the workflow, I might need to define more of the coordination logic myself. CrewAI's role-based structure was useful for this assignment because I could change the Technical Writer's backstory and observe its effect without redesigning the whole workflow.

## 5. Verification and AI use

I checked that the workflow completed and produced the output files. I compared the original and changed explanations to assess whether the writing style followed the new instructions. Because the kit does not access the web, I understand that generated factual claims may need independent verification.

I used ChatGPT to help troubleshoot setup issues, understand the code, and prepare the report. I checked the commands and project outputs in my own environment. The generated explanations should still be reviewed for factual accuracy before being treated as reliable information.