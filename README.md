# best-practices

## General

- 

## Github

- Use [the projects board](https://github.com/orgs/passiondynamics/projects) to find tickets to pick up/implement.
- The ticket should be in `Ready` to be picked up and moved along the different states as it progresses.
- Each ticket should(/will probably) have one corresponding PR. Conversely, each PR should be for one ticket/feature.
  The idea for PRs are minimal changes that add one new thing to the application.

## Code

- Start off with "put in your best effort into writing good code". Subjective for now, but will append explicit
  practices as we go.
- Each repository should use a virtual environment/package manager/dependency framework. Examples of what we mean:
  - Python's `pipenv`/`pip`,
  - npm's `package.json`,
  - Rust's `Cargo.lock`,
  - Java's Gradle or Maven, and
  - etc.
