# Alternatives to Postman for Exploratory and Automated API Testing

Postman is a great tool for exploratory API Testing. However, it is not the best tool for automated API system testing and there will be a [change in September which can result in higher costs for using Postman](https://blog.postman.com/announcing-new-lightweight-postman-api-client/). In this blog post, I will explain why code based open source tools are often better for automated API system testing than GUI based tools like Postman or Insomnia. I will also provide some recommendations which tool to use for which technology stack.

System Testing against the API layer is a vital part of software development, as it ensures that the APIs are functioning correctly and meeting the expected requirements. However, not all API testing tools are created equal. In this blog post, I will compare and contrast two types of API testing tools: code based open source tools and GUI based tools like Postman or Insomnia. While Postman and Insomnia have both value in the context of exploratory API Testing - I will argue that code based open source tools are better for automated API system testing, especially in terms of maintainability and integration into existing development infrastructures.

## What are code based open source tools for API system testing?

Code based open source tools are API testing tools that allow the user to write and execute test scripts using a programming language, such as Java, Python, JavaScript, etc. Some examples of code based open source tools are [REST-Assured](https://rest-assured.io/),  [Karate](https://github.com/karatelabs/karate), [supertest](https://www.npmjs.com/package/supertest) and [PyTest](https://docs.pytest.org/en/7.4.x/). 

## What are GUI based tools like Postman or Insomnia for exploratory API Testing?

GUI based tools like [Postman](https://www.postman.com/) or [Insomnia](https://github.com/Kong/insomnia) are API testing tools that provide a graphical user interface (GUI) for the user to create and run test requests using a point-and-click approach. These tools are popular among developers and testers, as they offer a user-friendly and intuitive interface. I also use them heavily for exploratory API testing. Some features of these tools include:

- Support for various authentication methods
- Ability to create and manage collections of requests
- Built-in support for API documentation
- Wide range of integrations and plugins

### Postman versus Insomnia Licesing Model

Based on my research, Insomnia and Postman have different licensing models. Insomnia is an open-source, cross-platform API client that is free to use and modify. However, it also offers a paid plan that provides more features and support. Postman is a commercial API platform that offers a free plan for individual users and small teams, and [paid plans for larger teams and enterprises](https://www.postman.com/pricing/). Besides, there are many other alternatives like Paw, plugins for VSCode or IntelliJ. 

Both tools have their pros and cons, depending on your needs and preferences. Some factors to consider when choosing an API testing tool are:

- The features and functionalities that you require for your API development and testing
- The level of collaboration and integration that you need with other colleagues, tools and systems
- The budget and resources that you have available for the tool
- The user interface and experience that you prefer

## Why are code based open source tools better for automated API system testing?

While GUI based tools like Postman or Insomnia have their advantages, they also have some limitations when it comes to automated API system testing. Automated API system testing is the process of running a set of test cases repeatedly and automatically to verify the functionality, performance, and security of the APIs. This process is essential for ensuring the quality and reliability of the software.

Code based open source tools are better for automated API system testing for the following reasons:

- **Maintainability**: Code based open source tools allow the user to write test scripts using a programming language, which gives them more control and flexibility over the test logic and flow. This makes it easier to maintain and update the test scripts as the APIs change or evolve. On the other hand, GUI based tools like Postman or Insomnia rely on a graphical interface, which can be cumbersome and prone to errors when dealing with complex or dynamic scenarios. Moreover, code based open source tools can leverage existing frameworks and libraries that provide reusable and modular code components, which can improve the readability and maintainability of the test scripts.
- **Integration**: Code based open source tools can be easily integrated with other tools and systems, such as continuous integration (CI), continuous delivery (CD), version control, reporting, etc. This can enhance the automation and collaboration capabilities of the testing process. GUI based tools like Postman or Insomnia have some extensibility features, but they are not as comprehensive or customizable as code based open source tools.
- **Cost-effectiveness**: Code based open source tools are free and open source, meaning that anyone can use them without paying any fees or licenses. This can save a lot of money and time for the users, as they do not have to worry about purchasing or renewing subscriptions or licenses. GUI based tools like Postman or Insomnia have free versions, but they also have paid plans that offer more features and functionalities. Sometimes these paid plans can be quite expensive or the license come with changes of terms and conditions that can be problematic for the users. Test code can be as important as productive code. You need to consider that for some products the code will need to be maintained for many decades. Sometimes the test code even outlives the productive code, since it contains the domain knowledge in the format of tests. This can remain relevant even if you rewrite the productive code. With 3rd party tools, there comes a risk and a dependency to the supplier including licensing issues. Therefore, for test code you should prefer open source tools over 3rd party tools. 

## Further benefits mentioned by teams after migrating to code-based tools for automation

The following further disadvantages of a Postman setup were mentioned by teams after migrating to code-based tools for automation:

- High complexity of test sequences and scripts in Postman / Newman  Poor maintainability, unstable execution
- No IDE integration of Postman: different environment for developing these tests compared to the rest of the code.
- Lack of GitHub integration of test code  no normal working with PRs and code review in PR etc. possible
- The common approach to store collections externally in the cloud can be incompliant with company policies. On the other hand,  sharing code instead in an repository is transparent and compliant

## Recommendations: Alternative for Postman and Insomnia for Automated System Testing

### Recommendations: Alternative for Postman and Insomnia for Automated System Testing

For Automated System Testing against the API layer, you can use the tool, which is fitting best for your technology stack. Below some code based Open Source recommendations for the respective technology stacks - the list is not exclusive and there are further similar Open Source alternatives.

- Java
    - [Karate](https://github.com/karatelabs/karate)
    - [RestAssured](https://rest-assured.io/)
- JavaScript
    - [Mocha](https://mochajs.org/) or [Jest](https://jestjs.io/) NodeJS test frameworks
    - [Supertest](https://www.npmjs.com/package/supertest) HTTP client library
- Python
    - [Pytest](https://docs.pytest.org/en/7.4.x/) Test framework
    - [Requests](https://pypi.org/project/requests/) HTTP  client library
- ABAP
    - Either leveraging one of the above tools or writing system test with ABAP unit.

### Migration from Postman to Karate

For Karate test tool there is also a migration [support for Postman](https://www.youtube.com/watch?v=XLAzUzln3kE&t=1456s) available.

## Conclusion

In conclusion, code based open source tools are better for automated API system testing than GUI based tools like Postman or Insomnia, especially in terms of maintainability. Code based open source tools offer more control, maintainability, flexibility, extensibility, and cost-effectiveness than GUI based tools. Therefore, I recommend using code based open source tools for your automated API system testing needs. And tools like Postman and Insomnia only for exploratory API testing. If Postman is becoming too expensive due to the changes in September, you can check out Insomnia for the exploratory API system testing case.

| Use Case            | Stack      | Recommended Solution                                                                                                                                         | Comment                                                                   |
|---------------------|------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------|
| Exploratory Testing | General    | [Insomnia](https://github.com/Kong/insomnia) or [Visual Studio Code plus REST Client](https://marketplace.visualstudio.com/items?itemName=humao.rest-client) | Choice depends on preference for GUI support or better integration in IDE |
| Test Automation     | Java       | [Karate](https://github.com/karatelabs/karate) or [RestAssured](https://rest-assured.io/)                                                                    | Choice depends on existing technology stack                               |
|                     | JavaScript | [Mocha](https://mochajs.org/) or [Jest](https://jestjs.io/), [Supertest](https://www.npmjs.com/package/supertest) - HTTP client library                      | Choice depends on existing technology stack                 |
|                     | ABAP       | Either leveraging JavaScript based tools or writing system test with ABAP unit.                                                                              | Choice depends on existing technology stack                               |  


## Resources

- [Testing Terminology: System Testing](https://ecosystem4engineering.substack.com/p/shared-language-for-talking-about)
- [Visual Studio Code plus REST Client](https://marketplace.visualstudio.com/items?itemName=humao.rest-client)
- [JetBrains PyCharm plus HTTP client](https://www.jetbrains.com/help/idea/2022.1/http-client-in-product-code-editor.html)
- [Plugin for Postman to Karate migration](https://www.youtube.com/watch?v=XLAzUzln3kE&t=1456s)


## Related Blogs on Test Automation

You can find more information about test automation in the following blogs:
- [Get Higher Quality and Productivity by tackling the Broken Window Effect](https://ecosystem4engineering.substack.com/p/get-higher-quality-and-productivity)
- [The hidden cost of flaky tests](https://ecosystem4engineering.substack.com/p/the-hidden-costs-of-flaky-tests)
- [Why a maintainable and readable test suite is important to stay agile](https://ecosystem4engineering.substack.com/p/adaptability-and-confidence-to-change)
