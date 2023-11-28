### Conceptual Exercise

Answer the following questions below:

- What is a JWT?
  - A JWT comprises a header, payload, and signature within a string.
    - Its purpose is to securely store data that can be verified at a subsequent stage through signature validation.

- What is the signature portion of the JWT?  What does it do?
  - Authenticated using a confidential key, the signature is specific to a particular header and payload, employing a designated algorithm specified in the header.

- If a JWT is intercepted, can the attacker see what's inside the payload?
  - Yes. You shouldn't store sensitive info in a JWT.

- How can you implement authentication with a JWT?  Describe how it works at a high level.
  -  Initiate the request by providing a username and password. Upon successful authentication, the server responds with a token encoded and signed using the standard JWT format. The front-end receives and retains this token in local storage. Subsequently, for each future request, the browser sends this token to the server.

- Compare and contrast unit, integration and end-to-end tests.
  - Integration testing involves integrating small code increments, rejecting the code if tests fail.
  - Unit testing entails evaluating individual code components, such as the functionality of a specific function.

- What is a mock? What are some things you would mock?
  - Developing a simulated version of an external or internal service to substitute for the actual one enhances the efficiency and reliability of your tests. This practice is often employed in unit testing. When an object under test relies on dependencies with other (complex) objects, using mocks to mimic their behavior helps isolate the specific behavior. This proves beneficial when incorporating the real objects into the unit test is impractical.

- What is continuous integration?
  - Continuous Integration is the practice of merging in small code changes frequently, rather than merging in a large change at the end of a development cycle.

- What is an environment variable and what are they used for?
  - A variable with a value set externally to the program, usually inherent to the operating system. Comprising a name/value pair, any number of such variables can be generated and accessed at a given point in time.

- What is TDD? What are some benefits and drawbacks?
  - Test-Driven Development (TDD) is a testing approach where tests are authored before the actual code. After creating the tests, the application code is then developed. This method encourages the creation of a meticulously planned app with a primary focus on testing. However, it typically extends the overall time required for completion.

- What is the value of using JSONSchema for validation?
  - Enables rapid identification of user data issues before reaching the database, minimizes the code needed for data processing and validation, and establishes a straightforward and maintainable validation system.

- What are some ways to decide which code to test?
  - Verify checkpoints that a user encounters while navigating through the application. Assess various outcomes associated with the user experience. Ensure that the app is working as intended.

- What does `RETURNING` do in SQL? When would you use it?
  - RETURNING will return the data that was inserted, updated, or deleted in SQL.

- What are some differences between Web Sockets and HTTP?
  - HTTP is a heavy protocol and is stateless. Ask for answer, get answer, hang up connection.
  - Websockets are tiny and stateful often used to tell the browser something has changed. They stay connected.

- Did you prefer using Flask over Express? Why or why not (there is no right
  answer here --- we want to see how you think about technology)?
  - I lean towards utilizing Python/Flask for backend development. The workflow seems more streamlined and straightforward. 
  - Express, in comparison, appears more cumbersome and demands more effort for achieving a comparable result.