Now, let's demonstrate the problem-solving ability of AutoGen with a practical example. Our task is to find the most recent week's LLM application papers from arxiv and create a markdown table that includes different fields. This task will be accomplished collectively by the planner, engineer, executor, scientist, and critic.

**Planner**: The primary task of the planner is to propose a detailed plan. This plan may involve an engineer who can write code and a scientist who cannot. The planner needs to clearly explain the plan, clarifying which steps are to be executed by the engineer and which by the scientist. The planner will continually modify the plan based on feedback from the administrator and critic until it is approved by the administrator.

**Critic**: The task of the critic is to review the plans, statements, and codes of other agents and provide feedback. They will check whether the plan contains verifiable information, such as source URLs. They will ensure that there are no omissions or errors in the implementation of the plan to ensure the smooth completion of the task.

**Scientist**: The scientist will follow the approved plan. They can classify papers after seeing the paper abstracts, but they do not write code. Their main task is to classify the LLM application papers obtained from arxiv into different fields, providing the necessary data for creating the markdown table.

**Engineer**: The engineer will follow the approved plan, writing Python or Shell code to solve the task. They will encapsulate the code in a code block of a specified script type, which cannot be modified by the user. Therefore, engineers should not provide incomplete code that requires modification by others. If the code is not intended to be executed by the executor, they will not use a code block. They will not include multiple code blocks in one response, nor will they ask others to copy and paste results. Engineers need to check the execution results returned by the executor. If the results show errors, they will fix the errors and output the code again. They will provide complete code, not partial code or code changes. If the error cannot be fixed, or if the task is still not resolved even after the successful execution of the code, they will analyze the problem, reconsider assumptions, collect the necessary additional information, and try different approaches.

**Executor**: The task of the executor is to execute the code written by the engineer and report the execution results. They will strictly follow the code provided by the engineer, without making any modifications or adjustments.





