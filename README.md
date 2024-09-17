Thank you! Below is the Prompt Engineering Guide formatted in Markdown. You can copy and paste this into a `.md` file for easy reading and sharing.

---

# Prompt Engineering Guide

**Note:** This guide consolidates key principles and best practices in prompt engineering, drawing on recent advances and insights from industry leaders like Anthropic and OpenAI. While some information may align with established practices, the aim is to provide a comprehensive resource that enhances your ability to craft effective prompts. Understanding the inner workings of large language models (LLMs) is crucial for guiding their behavior to produce desired outcomes.

## Introduction and General Concepts

Prompt engineering is the process of designing and structuring prompts to guide AI models in generating accurate, relevant, and useful responses. Effective prompts serve as clear instructions that help the AI understand the task, context, and desired output. In models like OpenAI's GPT-4 and Anthropic's Claude, the way you phrase your prompt can significantly influence the model's reasoning, ethics, and style of response.

Key aspects of prompt engineering include:

- **Clarity:** Providing unambiguous instructions.
- **Context:** Supplying background information to frame the task.
- **Specificity:** Defining precise requirements and constraints.
- **Ethical Guidelines:** Ensuring the AI adheres to ethical standards and avoids biases.
- **Iterative Refinement:** Continuously improving prompts based on AI feedback.

By mastering these concepts, you can leverage AI models more effectively for tasks ranging from answering questions and generating creative content to problem-solving and data analysis.

## Guidelines

1. **Define the AI's Role Clearly:**
   - **Explanation:** Specify the role or persona the AI should assume to provide context and guide its responses.
   - **Example:** "You are a medical doctor specializing in cardiology."

2. **Provide Relevant Context:**
   - **Explanation:** Include necessary background information to help the AI understand the task fully.
   - **Example:** "Given the rising trend of remote work due to recent global events..."

3. **Be Specific with Instructions:**
   - **Explanation:** Clearly state what you want the AI to do, including any steps or considerations.
   - **Example:** "Summarize the key points of the following article in three bullet points."

4. **Set the Desired Tone and Style:**
   - **Explanation:** Indicate the tone (formal, informal) and style (technical, conversational) you want in the response.
   - **Example:** "Explain the concept in a friendly, conversational manner suitable for beginners."

5. **Limit the Scope:**
   - **Explanation:** Define boundaries to focus the AI's response on specific areas.
   - **Example:** "Discuss renewable energy sources, excluding solar power."

6. **Encourage Step-by-Step Reasoning:**
   - **Explanation:** Prompt the AI to think through problems logically and sequentially.
   - **Example:** "Explain each step of the process to solve this equation."

7. **Specify the Format:**
   - **Explanation:** Request a particular structure, such as lists, tables, or essays.
   - **Example:** "Provide the information in a table format with columns for advantages and disadvantages."

8. **Avoid Ambiguity:**
   - **Explanation:** Use clear and precise language to prevent misunderstandings.
   - **Example:** Instead of "Tell me about banks," specify "Describe the role of central banks in the economy."

9. **Instruct on Handling Uncertainty:**
   - **Explanation:** Guide the AI on what to do if it's unsure about an answer.
   - **Example:** "If you are uncertain, please state that the information may be incomplete."

10. **Address Ethical and Sensitive Topics Appropriately:**
    - **Explanation:** Instruct the AI to handle sensitive subjects with care and neutrality.
    - **Example:** "Discuss the impact of immigration policies without bias."

11. **Avoid Unnecessary Apologies:**
    - **Explanation:** The AI should focus on providing helpful information rather than apologizing for limitations.
    - **Example:** Instead of "I'm sorry, but I cannot...," use "I cannot provide that information, but I can help with..."

12. **Use Positive Language:**
    - **Explanation:** Frame instructions positively to encourage constructive responses.
    - **Example:** "Describe effective time management strategies" instead of "Don't talk about ineffective strategies."

13. **Set Knowledge Cutoff Dates:**
    - **Explanation:** Specify if you need information up to a certain date to ensure relevance.
    - **Example:** "As of October 2023, what are the latest developments in renewable energy?"

14. **Encourage Creativity and Originality:**
    - **Explanation:** Invite the AI to generate unique ideas or solutions.
    - **Example:** "Propose an innovative marketing strategy for a new tech startup."

15. **Ask for Multiple Perspectives:**
    - **Explanation:** Request the AI to consider different viewpoints or solutions.
    - **Example:** "Analyze the benefits and drawbacks of artificial intelligence in healthcare."

16. **Use Examples to Clarify:**
    - **Explanation:** Provide examples within your prompt to illustrate what you're asking for.
    - **Example:** "Generate a metaphor to explain cloud computing, such as 'It's like renting space in someone else's warehouse.'"

17. **Instruct to Cite Sources When Necessary:**
    - **Explanation:** Ask the AI to provide references for factual information.
    - **Example:** "List the statistics on global warming with their sources."

18. **Break Down Complex Tasks:**
    - **Explanation:** Encourage the AI to divide large problems into manageable parts.
    - **Example:** "Outline the steps needed to implement a new software system in an organization."

19. **Use Tags or Headings for Organization:**
    - **Explanation:** Structure your prompt with headings to separate different instructions.
    - **Example:**

      ```
      [Objective]: ...
      [Constraints]: ...
      [Format]: ...
      ```

20. **Confirm Understanding:**
    - **Explanation:** Ask the AI to summarize or restate the instructions to ensure comprehension.
    - **Example:** "Before proceeding, please summarize the task in your own words."

21. **Keep Augmented Context in Mind:**
    - **Explanation:** often the context required to answer requires precise information in order to reach the correct answer, if those can be found online (and the model allows it) just specify to browse for it. Otherwise you need to provide it in other ways (ie. RAG)
    - **Example:** "What is ____, feel free to browse."

22. **Multi-step process:**
    - **Explanation:** certain tasks can't be performaed with one prompt and one model, you can use several iteration in order to reach the prompt that allows another model to complete the task
    - **Example:** gpt-4 "Browse all the info about X and summarize it in a organized fashion using markdown format." then to o1 ""Find out [...] using the following info [paste from previous model]"

## Tips

1. **Start with a Simple Prompt and Build Upon It:**
   - Begin with a basic prompt and add details incrementally to refine the response.

2. **Experiment with Different Phrasings:**
   - Reword your prompt if the AI doesn't provide the desired output.

3. **Use Open-Ended Questions for Elaborate Responses:**
   - Encourage detailed answers by avoiding yes/no questions.

4. **Provide Examples in Your Prompt:**
   - Illustrate the desired output to guide the AI.

5. **Specify the Intended Audience:**
   - Tailor the complexity and language style to suit the audience.
   - **Example:** "Explain the theory to a group of middle school students."

6. **Set Length Constraints if Needed:**
   - Control the verbosity of the response.
   - **Example:** "Summarize the article in approximately 150 words."

7. **Encourage the Use of Analogies:**
   - Help simplify complex topics.
   - **Example:** "Explain blockchain technology using an analogy related to a ledger."

8. **Request a Particular Point of View:**
   - Instruct the AI to write from a specific perspective.
   - **Example:** "Write an opinion piece on climate change from the viewpoint of an environmental activist."

9. **Ask for Clarification if the Response is Unclear:**
   - If the AI's answer is ambiguous, prompt it to elaborate.

10. **Iterate Based on Feedback:**
    - Use the AI's response to adjust your prompt for better results.

## Examples

Below are examples that demonstrate how to apply the guidelines and tips effectively, each referencing specific guidelines and tips.

### Example 1: Defining Role and Providing Context (Guidelines 1 & 2, Tips 5 & 4)

- **Prompt:** "You are a historian specializing in ancient civilizations. Explain the significance of the Rosetta Stone to a group of college students."

- **Analysis:**
  - **Defines Role (Guideline 1):** "You are a historian specializing in ancient civilizations."
  - **Provides Context (Guideline 2):** "Explain the significance of the Rosetta Stone."
  - **Specifies Audience (Tip 5):** "To a group of college students."
  - **Be Specific with Instructions (Guideline 3):** Focus on the Rosetta Stone's significance.

### Example 2: Encouraging Step-by-Step Reasoning (Guideline 6, Tip 1)

- **Prompt:** "Step-by-step, calculate the total interest earned on a $5,000 investment over 3 years at an annual interest rate of 5% compounded annually."

- **Expected Response:**
  1. **Year 1:** Interest = $5,000 * 5% = $250; New Total = $5,250.
  2. **Year 2:** Interest = $5,250 * 5% = $262.50; New Total = $5,512.50.
  3. **Year 3:** Interest = $5,512.50 * 5% = $275.63; New Total = $5,788.13.
  4. **Total Interest Earned:** $5,788.13 - $5,000 = **$788.13**.

- **References:**
  - **Encouraging Step-by-Step Reasoning (Guideline 6).**
  - **Start Simple and Build (Tip 1).**

### Example 3: Specifying Format and Limiting Scope (Guidelines 7 & 5, Tip 6)

- **Prompt:** "In a table format, compare the key features of electric cars and hybrid cars, focusing only on environmental impact and cost."

- **Expected Response:**

  | Feature              | Electric Cars                                                                                   | Hybrid Cars                                                                                          |
  |----------------------|-------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|
  | **Environmental Impact** | - Zero tailpipe emissions<br>- Reduces greenhouse gases if electricity is from renewable sources | - Lower emissions than traditional cars<br>- Higher emissions than electric cars due to gasoline use |
  | **Cost**                 | - Generally higher upfront cost<br>- Lower maintenance and fuel costs over time                | - Moderate upfront cost<br>- Fuel savings compared to traditional cars but less than electric cars   |

- **References:**
  - **Specify the Format (Guideline 7).**
  - **Limit the Scope (Guideline 5).**
  - **Use Examples to Clarify (Tip 4).**

### Example 4: Handling Sensitive Topics (Guideline 10, Tip 5)

- **Prompt:** "Discuss the ethical considerations of genetic editing in humans, ensuring an unbiased perspective suitable for a graduate-level audience."

- **Expected Response:**
  - **Ethical Considerations:**
    - **Pros:**
      - Potential to eliminate genetic diseases.
      - Can improve quality of life.
    - **Cons:**
      - Risks of unintended consequences.
      - Moral concerns about 'playing God.'
  - **Conclusion:** Ongoing debate requires careful consideration of both scientific possibilities and ethical implications.

- **References:**
  - **Address Ethical and Sensitive Topics (Guideline 10).**
  - **Specify Intended Audience (Tip 5).**

### Example 5: Avoiding Ambiguity and Confirming Understanding (Guidelines 8 & 20, Tip 9)

- **Prompt:** "Calculate the final price after a 15% discount on an item that costs $200, and then add a 7% sales tax. Confirm each step."

- **Expected Response:**
  1. **Calculate Discount:** 15% of $200 = $30 discount.
  2. **Subtract Discount:** $200 - $30 = $170.
  3. **Calculate Sales Tax:** 7% of $170 = $11.90.
  4. **Add Sales Tax:** $170 + $11.90 = **$181.90**.
  5. **Final Price:** **$181.90**.

- **References:**
  - **Avoid Ambiguity (Guideline 8).**
  - **Confirm Understanding (Guideline 20).**

### Example 6: Encouraging Creativity (Guideline 14, Tip 2)

- **Prompt:** "Invent a new sport that combines elements of soccer and basketball, and describe how it is played."

- **Expected Response:**
  - **Name:** **Socketball**.
  - **Description:** Played on a rectangular court with goals at each end and hoops above them.
  - **Rules:**
    - Players use feet to move the ball like in soccer.
    - To score, players can:
      - Kick the ball into the goal (1 point).
      - Throw it through the hoop after catching it with their hands (2 points).
  - **Objective:** Encourages teamwork and versatility.

- **References:**
  - **Encourage Creativity and Originality (Guideline 14).**
  - **Use Open-Ended Questions (Tip 2).**

### Example 7: Asking for Multiple Perspectives (Guideline 15, Tip 8)

- **Prompt:** "Evaluate the impact of automation on employment, discussing both the positive and negative effects."

- **Expected Response:**
  - **Positive Effects:**
    - Increases efficiency and productivity.
    - Creates new job opportunities in tech sectors.
  - **Negative Effects:**
    - Displaces workers in certain industries.
    - May widen the skills gap.

- **References:**
  - **Ask for Multiple Perspectives (Guideline 15).**
  - **Request a Particular Point of View (Tip 8).**

### Example 8: Instructing to Cite Sources (Guideline 17, Tip 4)

- **Prompt:** "Provide three recent statistics on cybersecurity threats, citing reputable sources."

- **Expected Response:**
  1. "In 2023, cybercrime is expected to cost the world $10.5 trillion annually. *(Source: Cybersecurity Ventures)*"
  2. "Ransomware attacks increased by 150% in the first half of 2023. *(Source: ABC Cybersecurity Report)*"
  3. "Over 70% of businesses are not prepared for a cyber attack. *(Source: XYZ Security Survey)*"

- **References:**
  - **Instruct to Cite Sources (Guideline 17).**
  - **Provide Examples in Your Prompt (Tip 4).**

### Example 9: Breaking Down Complex Tasks (Guideline 18, Tip 1)

- **Prompt:** "Outline the steps needed to plan a successful product launch for a new smartphone."

- **Expected Response:**
  1. **Market Research:** Analyze target audience and competitors.
  2. **Product Development:** Finalize features and design.
  3. **Marketing Strategy:** Develop branding and promotional materials.
  4. **Logistics Planning:** Ensure supply chain and distribution channels are ready.
  5. **Launch Event:** Organize press releases and launch events.
  6. **Post-Launch Support:** Set up customer service and gather feedback.

- **References:**
  - **Break Down Complex Tasks (Guideline 18).**
  - **Start Simple and Build Upon It (Tip 1).**

### Example 10: Using Tags for Organization (Guideline 19, Tip 4)

- **Prompt:**

  ```
  [Role]: Financial Analyst
  [Task]: Assess the financial viability of investing in renewable energy stocks.
  [Constraints]: Focus on data from the last five years.
  [Format]: Provide a summary followed by recommendations.
  ```

- **Expected Response:**
  - **Summary:**
    - Renewable energy stocks have shown consistent growth over the past five years, with an average annual return of X%.
  - **Recommendations:**
    - **Positive Outlook:** Due to global shifts towards sustainability.
    - **Considerations:** Market volatility and regulatory changes.
    - **Conclusion:** Investing in renewable energy stocks appears financially viable with a long-term perspective.

- **References:**
  - **Use Tags or Headings for Organization (Guideline 19).**
  - **Specify the Format (Guideline 7).**

### Example 11: Confirming Understanding (Guideline 20, Tip 9)

- **Prompt:** "Before solving, summarize this problem in your own words: 'A cyclist travels at an average speed of 15 km/h for 2 hours and then increases the speed to 20 km/h for the next 1.5 hours. What is the total distance covered?'"

- **Expected Response:**
  - **Summary:** "You want me to calculate the total distance a cyclist covers by first riding 15 km/h for 2 hours and then 20 km/h for 1.5 hours."
  - **Solution:**
    1. **First Part:** 15 km/h * 2 hours = 30 km.
    2. **Second Part:** 20 km/h * 1.5 hours = 30 km.
    3. **Total Distance:** 30 km + 30 km = **60 km**.
  - **Answer:** The cyclist covers a total of **60 km**.

- **References:**
  - **Confirm Understanding (Guideline 20).**
  - **Ask for Clarification (Tip 9).**

### Example 12: Handling Uncertainty (Guideline 9, Tip 3)

- **Prompt:** "Who is predicted to win the next presidential election?"

- **Expected Response:**
  - "As of my last update in September 2023, I cannot predict future election outcomes. Election results depend on various factors and can be influenced by ongoing events."

- **References:**
  - **Instruct on Handling Uncertainty (Guideline 9).**
  - **Specify Knowledge Cutoff Dates (Guideline 13).**
