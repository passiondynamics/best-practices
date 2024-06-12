## Code

- Start off with "put in your best effort into writing good code". Subjective for now, but will append explicit
  practices as we go.
- Each repository should use a virtual environment/package manager/dependency framework. Examples of what we mean:
  - Python's `pipenv`/`pip`,
  - npm's `package.json`,
  - Rust's `Cargo.lock`,
  - Java's `Gradle` or `Maven`,
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
- Comment your code! Explain something to future-you when you look back at this complex logic you fever-dreamed up and
  won't understand why you wrote it like this.
  - Once you get a hang of it, the next level is less: commenting what's going on, and more: **why** it's written this
    way. More experienced developers can read your code and figure out what it's actually doing, but understanding why
    it has to work this way instead of some other way is something you can shed a lot of light on.
- Never hardcode secrets! That includes API keys, tokens, or any sensitive strings that would give access to something you
  don't want a determined actor to have.
