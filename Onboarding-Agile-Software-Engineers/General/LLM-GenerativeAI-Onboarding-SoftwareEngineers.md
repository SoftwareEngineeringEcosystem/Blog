# Leveraging Generative AI

Generative AI can be a valuable to enhance productivity and make things possible, which you were not capable before. At the same time there are also several challenges when using generative AI or building applications integrating generative AI.

This page shall summarize some important principles to consider and provide and overview of the past sessions.

## First Principles

Generative AI allows to create a lot of content and code quickly, sometimes the quality of the result can be surprisingly good, but the quality can also be pretty bad. The tools can also be used in a wrong way to optimize towards certain KPIs.
E.g. we have seen tools which help to create test case automatically to cover the code coverage targets, which misses the actual goal of achieving code coverage with effective tests.

Based on these observation we want to create a common understanding and alignment with some guiding principles for using the tools in a responsible way:
- **Responsible Developer:** As a developer use the tools in a responsible way and ensure that the productive code and test code are of high quality, secure, maintainable, readable and testable. Do not bring AI generated code into production without human review.
- **Quality Mindset:** Assume that there are problems in the generated code: Generative AI, particularly the large-scale generative language models, have the capacity to produce diverse, creative, and contextually relevant content. However, the potential for the AI to generate text that deviates from facts or lacks coherence, known as hallucinations, necessitates the development of strategies to ensure the quality of generated content.
- **Consider Security:** New capabilities often also create new security attack vectors. When integrating generative AI, take care of prompt injection.
- **Experiment:** Experiment with using generative AI for all kinds of tasks. Be curious. Not only try to achieve the same in a more productive way, but also explore new capabilities allowing you to have greater impact and be more effective.
- **Abundance Mindset over Productivity Improvements:** Think about what additional things it enables you to do instead of thinking only about how to do existing tasks faster.
- **Leverage Multiple Tools:** Ensure you integrate automated tools for security scanning, code quality and code formatting in your development process.
- **Adopt new practices, some old practices will become less effective:** E.g. if code coverage can easily be achieved by generating tests, new practices like leveraging mutation testing can become relevant.


## Course Offering

If you want to get started and learn more about how to develop applications on top of generative AI, you can also check out the following course offering.

The ChatGPT Prompt Engineering for Developers course, offered by deeplearning.ai, aims to equip developers with the knowledge and skills required to effectively utilize OpenAI's ChatGPT. The course covers essential topics such as understanding ChatGPT, designing user prompts, utilizing transformations, tokens, models, and output diversity, refining prompts into task-based templates, and overcoming biases and common pitfalls in the engagement process. This course ultimately helps developers create more versatile and accurate AI language models to address a range of use cases.

It also touches how to leverage libraries like LangChain.

https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/

There is also a course offered by [Hasso Plattner Institute in German](https://open.hpi.de/courses/kizukunft2023) in German, which is kind of a first introduction into the topic. Suited for colleagues without a software engineering background.

### Documentation

- [GPT Best Practices](https://platform.openai.com/docs/guides/gpt-best-practices)
- [OWASP Top 10 for LLM Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/): A standard awareness document for developers and web application security that provides a concise description of prompt injection and other common and critical security risks to LLM applications.
- [Learn Prompting - Defensive Measures](https://learnprompting.org/docs/category/-defensive-measures): A collection of resources and best practices for mitigating prompt injection attacks.
- [Emerging Technology Stacks and Architecture](https://ecosystem4engineering.substack.com/p/impact-of-generative-ai-on-software) - reference architecture for the emerging LLM app stack, showcasing common systems, tools, and design patterns


