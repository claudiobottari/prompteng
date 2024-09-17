## Anthropic Claude System Prompts
Recently, I reviewed Anthropic Claude's approach to system prompts and here are the highlights...

# Prompt Engineering Guide
**Note:** These notes are derived directly from the analysis of Anthropic's system prompts, as it represents one of the most recent and reliable sources on the topic. That said, much of this information is not groundbreaking and aligns with established best practices in the field. In my view, prompt engineering is 90% common sense, especially when one has a solid understanding of how large language models (LLMs) function. The key principles often become clear once the inner workings of these models are grasped.

## INTRODUCTION AND GENERAL CONCEPTS
Prompt engineering is the process of designing and structuring prompts that guide AI models to produce desired responses. In the context of AI models like Claude 3 and its variations, creating effective prompts is essential for improving the quality, precision, and usefulness of the output. Anthropic has demonstrated their approach by releasing their system prompts, which provide a framework for how their models function, offering valuable insights into how to structure prompts for similar systems.

Effective prompt engineering involves not only specifying what the model should do but also ensuring that it adheres to certain guidelines, ethical standards, and strategies for handling complex or sensitive queries. A well-structured prompt can significantly improve the model’s behavior, ensuring concise answers for simple tasks and in-depth responses for more complicated or open-ended tasks.

## GUIDELINES
1. **Transparency:** Share how prompts or system updates affect model behavior to foster trust.
2. **Role Definition:** Clearly define the role the AI model plays within the conversation.
3. **Knowledge Cutoff:** Explicitly specify the model’s knowledge cutoff date to limit its information and avoid confusion.
4. **Concise for Simple, Thorough for Complex:** Guide the model to provide concise responses for simple queries and detailed ones for complex ones.
5. **Markdown for Coding:** Ensure that code responses are formatted using markdown for clarity.
6. **No Apologies for Inability to Perform Tasks:** Avoid unnecessary apologies; simply state limitations or refusals.
7. **Hallucination Alerts:** If unsure, the model should alert users that the information may not be reliable (hallucination).
8. **Tagging for Structured Prompts:** Use tags to structure the prompt and provide the model with specific sets of instructions.
9. **Objective and Ethical Handling of Sensitive Topics:** Ensure neutrality and avoid bias when dealing with controversial subjects.
10. **Chain-of-Thought Reasoning:** For complex tasks, guide the model to think step by step to improve accuracy.
11. **Clarify Before Acting on Visual Inputs:** If images are involved, ensure the model confirms its understanding before proceeding.
12. **Repetition of Key Instructions:** Repeat important instructions within the prompt to reinforce behavior.
13. **Break Down Large Tasks:** When a query requires a large output, break it into smaller tasks and ask for feedback from the user.

## TIPS
1. **Emphasize Transparency:** Provide detailed explanations for how the system works and any changes made (related to Guideline 1).
2. **Explicit Cutoff Dates (only for Claude):** Specify knowledge cutoffs to prevent outdated or misleading information (Guideline 3).
3. **Structure with Tags (only for Claude 3.5 Sonnet):** Organize the prompt with tags to ensure clarity and systematic responses (Guideline 8).
4. **Provide Context:** Give the AI context to help it understand its role and the type of response needed (Guideline 2).
5. **Repeat Important Instructions (only for Claude):** Reinforce key points through repetition to ensure compliance (Guideline 12).
6. **Incorporate Step-by-Step Thinking:** Use chain-of-thought prompting for tasks requiring logical progression (Guideline 10).
7. **Avoid Apologizing (only for Claude 3.5 Sonnet):** Instead of unnecessary apologies, instruct the model to simply explain limitations (Guideline 6).
8. **Acknowledge Potential Hallucinations:** When uncertain, the model should make users aware of possible inaccuracies (Guideline 7).
9. **Clarify Visual Inputs (only for Claude with images):** Ensure the model confirms image-based instructions before acting (Guideline 11).
10. **Offer Concise Answers First, Then Elaborate:** Start with brief responses for simple queries, but offer to provide more details when needed (Guideline 4).
11. **Use Markdown for Code Responses (only for Claude):** Ensure that any code snippets are formatted for clarity using markdown (Guideline 5).
12. **Handle Sensitive Topics Neutrally (only for Claude):** Maintain ethical and objective responses when discussing sensitive or controversial topics (Guideline 9).

## EXAMPLES
Here are a few examples to illustrate how these guidelines and tips can be applied:

1. **Handling Simple and Complex Queries (Guideline 4, Tip 10)**:
   - **Prompt Example**: "What is the population of France?" (Simple) vs. "Can you explain how the French healthcare system evolved?" (Complex)
   - **Result**: For the first query, the model gives a concise response with the population figure. For the second, the model provides a thorough historical explanation of healthcare reforms in France.

2. **Using Markdown for Coding (Guideline 5, Tip 11)**:
   - **Prompt Example**: "Can you write a Python function that adds two numbers?"
   - **Result**: The model outputs the code snippet in markdown format, making it easier to copy and execute:
     ```python
     def add_numbers(a, b):
         return a + b
     ```

3. **Hallucination Alerts for Uncommon Topics (Guideline 7, Tip 8)**:
   - **Prompt Example**: "Tell me about a rare species of bird found only in one remote part of the Amazon."
   - **Result**: The model provides an answer but ends with a caution: "This information may not be fully reliable as it's based on limited sources."

4. **Chain-of-Thought Reasoning for Problem Solving (Guideline 10, Tip 6)**:
   - **Prompt Example**: "Solve this math problem step-by-step: What is 25 times 43?"
   - **Result**: The model proceeds systematically:
     1. Breaks down the multiplication.
     2. Adds intermediate results.
     3. Provides the final answer.

5. **Clarifying Visual Inputs (Guideline 11, Tip 9)**:
   - **Prompt Example**: (User uploads an image) "Can you describe what this image shows?"
   - **Result**: The model clarifies: "The image contains a building, trees, and some people, but I cannot identify any specific individuals."

These examples highlight how structured, clear prompts, combined with specific techniques, improve the AI's performance in various scenarios.
