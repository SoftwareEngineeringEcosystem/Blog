# Clean Code: Writing maintainable, readable and testable code 

Clean code is a term used to describe software that is easy to read, understand, maintain and test. In this blog I want to summarize some important principles, provide an entry into the topic for beginners. Besides, the blog shall connect to the style guide repository, the books and current initiatives where experts can contribute. If you do not miss an update on clean code, test automation, communities of practice, decision making, testability and other engineering / craftsmanship / architecture topics, [subscribe to the brand new newsletter](https://ecosystem4engineering.substack.com/p/collaboration-on-improving).

## What makes code clean? 

Achieving clean code involves following a set of best practices and standards, such as using meaningful names, keeping functions small and focused, and using comments sparingly. Having a code base, which is readable and maintainable is essential for sustainable development. The books Clean Code from Robert C. Martin, Code Complete from Steve McConnell, The Pragmatic Programmer from David Thomas/Andy Hunt, and some other books contain many best practices and examples for clean code.

## What is code that’s not clean? 

Code that is not clean is code that is difficult to read, understand, and maintain. It may have poor organization, confusing or misleading names, inconsistent styling, and other issues that make it harder to work with.

Some examples of code that is not clean might include:
- Code with long, complex functions that are difficult to understand, test and maintain.
- Code with poor naming conventions, such as variables with short, non-descriptive names, or functions with names that do not accurately reflect their purpose.
- Code with inconsistent styling, such as inconsistent indentation or spacing, which can make it harder to read and understand.
- Code with unnecessary or redundant code, which can make it harder to maintain and understand.
- Code which making test automation hard, e.g. static coupling between classes.

Overall, code that is not clean is often more prone to errors and bugs, and can be more time-consuming to work with, as it requires more effort to understand, test and maintain.

![Code Quality from xkcd.com/1513/](resources/CleanCodeComic.png 'ABCDASDASDASDSDASDASD')

**Code Quality from xkcd.com/1513/ under [Creative Commons BY-ND 2.5](https://xkcd.com/license.html)**

## Benefits of Clean Code

There are many benefits to writing clean code, including:

- Improved readability and understandability: Clean code is easier to read and understand, which can make it easier for developers to adapt, debug, and maintain.
- Reduced risk of errors and bugs: Clean code is generally more reliable and less prone to errors and bugs, as it is easier to understand, test and maintain.
- Increased productivity: Clean code is easier and faster to work with, which can increase developer productivity and efficiency. According to a meta study [unhealthy code can contain more than 15 times more defects and reduce productivity by a factor of 9](https://www.linkedin.com/posts/klaus-h%C3%A4uptle-951a0349_according-to-a-meta-study-unhealthy-code-activity-6999048527821557760-mrWr?utm_source=share&utm_medium=member_desktop).
- Increased ability to adapt and evolve: Clean, modular code is easier to modify and update, which can help the software evolve and adapt to changing requirements over time.
- Improved team collaboration: Clean code is easier for team members to understand and work with, which can improve collaboration and communication within the team.
- Better long-term maintainability: Clean code is easier to maintain and update over time, which can save time and resources. And reduce risk if engineers move to other projects or leave the company.
- Increased code reuse: Clean, modular code is easier to reuse and repurpose in different contexts, which can save time and resources.
- Better performance: Clean code is generally more efficient and can run faster, as it is less complex and easier to optimize when needed.
- Improved code review process: Clean code is easier to review, as it is more organized and easier to understand. This can lead to more efficient and effective code reviews.
- Enhanced reputation: Writing clean code can help enhance the reputation of the developer or development team, as it demonstrates a commitment to quality and professionalism.

Overall, clean code can help ensure that your software is reliable, maintainable, and easy to work with, which can lead to increased efficiency, productivity, higher quality, and higher satisfaction of developers and users alike. The benefits of clean code extend beyond just the development process and can have a positive impact on the long-term success of the software and the team working on it.

## Important Clean Code Principles and Examples

First lets summarize some important principles for clean code and provide some simple examples. For every principle there is a lot more to learn in the style guide and the books.
- Clean code makes it easier for developers to understand, modify, and maintain a software system. When code is clean, it is easier to find and fix bugs, and it is less likely to break when changes are made. 
- One of the key principles of clean code is readability, which means that code should be easy to understand, even for someone who is not familiar with the system. To achieve this, developers should e.g. use meaningful names for variables, functions, and classes.
- Another important principle of clean code is simplicity, which means that code should be as simple as possible, without unnecessary complexity. To achieve this, developers should avoid using complex data structures or algorithms unless they are necessary, and should avoid adding unnecessary features or functionality.
- In addition to readability and simplicity, clean code should also be maintainable, which means that it should be easy to modify and update the code without breaking it. To achieve this, developers should write modular code that is organized into small, focused functions, and should avoid duplication of code.
- Finally, clean code should be well-documented. This means that it should include clear and concise comments that explain the purpose and functionality of the code. However, comments should not be used to explain the code itself; the code should be written in a way that is self-explanatory.

Overall, clean code is an essential part of software development. It makes it easier to understand and maintain a system, and can help to prevent bugs and other issues.

## The Style Guide Repository 

[https://github.com/SAP/styleguides](https://github.com/SAP/styleguides)

Under the CC BY 3.0 license and open to contributions from inside and outside of SAP, we hope that this repository will help developers worldwide to make their code a little cleaner, day by day.

The long term goal of the style guide repository is to cover the most important programming languages in the SAP world. So far only ABAP is covered, but I am convinced that more is to come. Maybe we will also be able to cover Java, TypeScript, Kotlin, Go and more - rather a wish than close to reality.

## The Books

There are several books, which cover the topic in detail, explain the reasoning and apply it to specific programming languages.
- [Clean ABAP](https://www.rheinwerk-verlag.de/clean-abap-a-style-guide-for-developers/)
- [Clean ABAP - German Version](https://www.rheinwerk-verlag.de/clean-abap-lesbarer-und-wartbarer-abap-code/)
- [Clean SAPUI5](https://www.sap-press.com/clean-sapui5_5479/)

The books are also very well suited for beginners or starters to learn the programming languages. Or colleagues who already mastered Clean ABAP and want to learn Clean SAPUI5. And even experts in the programming language mentioned that they learned a lot and it was a source of inspiration.

![Clean Code Book Family for ABAP and SAPUI5 / JavaScript](resources/cleancodeBookFamily.jpg 'Clean Code Book Family for ABAP and SAPUI5 / JavaScript')

**Clean Code Book Family for ABAP and SAPUI5 / JavaScript**

## A Foundation for Improvement

The main benefits of having a common understanding of a code style in a given programming language are improved maintainability, readability and testability. But there are also many other benefits and new possibilities, which this blog explores in more detail:

-   Why have a common set of rules? As an organization grows it helps to keep the **code base consistent and allows to let the developers focus on the important aspects**. There will be less conflicts about basics (e.g. formatting) due to a standard code style.
-   Fostering the principle of **optimizing code for the reader**: Given that code will be read far more often than it is written, an important principle for all rules is to optimize for the reader not the writer. Therefore the style guide weighs readability higher than using powerful expressions, which let the writer express something concisely, but are later hard to read.
-   Consistency of the code base: If the code base is built with the same principles and style guide in mind, it allows engineers to jump into an unfamiliar part of the code and **make improvements quickly**.
-   Improve Developer Experience: Having a consistent style guide **creates an ecosystem on its own and allows to improve the developer experience**. After the style guide was published in 2019, the community started to create tooling for improving code reviews, documented code review practices, extended static code checks, developed training formats and made some tooling to automatically correct code. This consistency created the foundation for several InnerSource / open source projects, platform improvements and triggered the exploration of further ideas.
-   Scaling an organization: As an organization grows it is important to have a common understanding of the code style. It helps to **ramp up new developers more quickly** and focus the time on pair programming or code reviews on other aspects.
-   Also **other roles -- not only developers -- benefit**, e.g. consultants who need to make extensions or SRE (Site Reliability Engineering) teams who need to improve operations.
-   The consistency also **improves the long-term maintenance** since new engineers taking the ownership can understand more quickly and maintain the code.
-   The style guide allows to **enforce rules with static code checks or even develop automatic corrections**. So some discussions do not take place anymore, which allows to focus the developers time on more important aspects..


## Current Activities

With the success of the style guide and number of improvement proposals there comes the need for a more formal process when it comes to reviewing improvement proposals. To make the whole process transparent and have clarity for making decisions.

This includes clarity on how those should be opened, are processed and the typical timeframe in which somehow can expect a decision. Besides, especially for changes with a larger impact (e.g. incompatible changes) we need a formal process for decision making, since those changes will also be reflected in static code checks and by that affect a large number of developers.

In the last months we have worked on documenting the whole process and written down our guiding principles for involving the community and making decisions. The process will soon be published. 

# Subscribe to Newsletter to stay informed

If you do not miss an update on clean code, test automation, communities of practice, decision making, testability and other engineering / craftsmanship / architecture topics, [subscribe to the brand new newsletter](https://ecosystem4engineering.substack.com/p/collaboration-on-improving). The newsletter will not only be used for sharing knowledge, but also offer opportunities for collaboration, building communities and co-creation.
