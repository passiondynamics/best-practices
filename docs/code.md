## Code

- Start off with "put in your best effort into writing good code". Subjective for now, but will append explicit
  practices as we go.
- Each repository should use a virtual environment/package manager/dependency framework. Examples of what we mean:
  - Python's `pipenv`/`pip`,
  - npm's `package.json`,
  - Rust's `Cargo.lock`,
  - Java's Gradle or Maven,
  - Go's built-in modules,
  - etc.
- Unit testing is required, and **good** unit testing is the bare minimum!
  - Lots of good resources already for how to write them, but the general structure I follow is that each unit test:
    ```
    1. Sets up arguments + other pre-conditions for a function call.
    2. Calls the function.
    3. Asserts the return value + other post-conditions are as expected.
    ```
  - High coverage is encouraged (80-95%).
  - Unit tests count as code too! They're just as important(/sometimes more than) as "regular" code, and so should also
    be treated as production code.
  - Some corresponding examples:
    - Java's `JUnit`
    - Python's `pytest`,
    - npm's `jest`,
    - Rust's and Go's built-in frameworks.
- Integration testing is required (except in special cases). Examples:
  - Python's `behave`
