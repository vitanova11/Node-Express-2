### Conceptual Exercise

Answer the following questions below:

- What is a JWT?
  JWT stands for JSON Web Token. It is a standard for securely transmitting information between two parties as a JSON object.

- What is the signature portion of the JWT? What does it do?
  The signature portion of the JWT is the version of header and payload signed with a secret key. It is the part that can't be decoded and proves that the person with the token is who they say they are.

- If a JWT is intercepted, can the attacker see what's inside the payload?
  Yes, if they decode it.

- How can you implement authentication with a JWT? Describe how it works at a high level.
  The token is created and signed on login, and then stored in the browser. For each request the token is sent from browser to server and validated.

- Compare and contrast unit, integration and end-to-end tests.
  Unit tests a single function, integration tests how functions work together, and end-to-end tests the entire user experience of the app. They are all similar in that they involve writing functions that tell the app to do something, and then compare the result with an expected result.

- What is a mock? What are some things you would mock?
  A mock is a simulated object or module that acts as a stand-in for a real object or module. Mocks are often used in testing to isolate the behavior of a particular module or component and to verify that it behaves as expected. A common example would be an API call.

- What is continuous integration?
  Continuous integration is the practice used by developers to regularly merge their code changes into a central repository, after which automated builds and tests are run. The key goals of continuous integration are to find and address bugs quicker, improve software quality, and reduce the time it takes to validate and release new software updates.

- What is an environment variable and what are they used for?
  An environment variable is a dynamic value that the operating system and other software can use to determine information specific to your computer. It is made up of a name/value pair and typically it is named in uppercase with words joined with an underscore (e.g., API_KEY). The primary use for environment variables is to separate the code and configuration, making it possible to use the same code in different environments. In other words, the environment in which the code runs can be configured independently of the code itself. This makes the code more reusable and easier to maintain.

- What is TDD? What are some benefits and drawbacks?
  Test Driven Development (TDD) is a software development practice that focuses on creating unit test cases before developing the actual code. It is an iterative approach combining programming, unit test creation, and refactoring. The primary intention of this technique is to modify or write new code only if the tests fail. The benefit of the TDD approach is that it aims to catch errors as early as possible in the development process, making debugging and fixing them easier. Traditional testing, however, may be more appropriate for larger and more complex projects where a more comprehenisive approach to testing is required.

- What is the value of using JSONSchema for validation?
  Using JSON Schema you can define rules and constraints that JSON data should adhere to. When your JSON documents adhere to these constraints it becomes easier to exchange structured data between applications because the data follows a consistent pattern. Without a standardized schema it becomes challenging to validate and enforce constraints on the data.

- What are some ways to decide which code to test?
  You should focus on testing the most complex and vulnerable parts of your code. Additionally, it is important to focus on testing the "behaviour" of your code as opposed to the implementation. You also want to focus on testing the most realistic use cases of your code.

- What does `RETURNING` do in SQL? When would you use it?
  The RETURNING clause allows you to retrieve values of columns that were modified by an insert, delete, or update. Without RETURNING you would have to run a SELECT statement after the DML statement is completed in order to obtain the values of the changed columns. So, you would use RETURNING to avoid unnecessary SQL statements in your database.

- What are some differences between Web Sockets and HTTP?
  HTTP is unidirectional where the client sends a request to the server and the server responds with the requested data. Web Sockets is a protocol that enables bidirectional, full-duplex communication between a client and a server over a single, long-lived connection. Web Sockets keep the connection between client and server open for as long as needed, allowing the server to send data to the client at any time without the need for the client to request it. The client can also send data to the server at any time.

- Did you prefer using Flask over Express? Why or why not (there is no right
  answer here --- we want to see how you think about technology)?
  I personally prefer Flask over Express because of its simplicity and ease of use. Flask also comes with a built-in development server and an interactive debugger. This feature is invaluable for developers as it allows for easy testing and debugging of applications during development. I think Flask is ideal for developing smaller applications as it allows for more control and is easier for beginners to pick up. Express is excellent for handling a multitude of concurrent requests, making it ideal for real-time applications.
