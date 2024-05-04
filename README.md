# best-practices

## General

- 

## Github

- Use [the projects board](https://github.com/orgs/passiondynamics/projects) to find tickets to pick up/implement.
- The ticket should be in `Ready` to be picked up and moved along the different states as it progresses.
- Each ticket should(/will probably) have one corresponding PR. Conversely, each PR should be for one ticket/feature.
  The idea for PRs are minimal changes that add one new thing to the application.

## Code

TL;DR: `Start off with "put in your best effort into writing good code". Subjective for now, but will append explicit
practices as we go.`

More [here](docs/code.md).

## Repository settings

See [here](docs/repo.md).

## Git

- Use descriptive commit messages!
  ```diff
  - "test fix"
  - "."
  - "comments"              <-- real commit messages from a teammate
  - "siuuuu"                <
  - "kjh,v,"                <
  - "begging on my knees"   <
  + "Add comments to call_server function"
  + "Update bundling mechanism to skip duplicates"
  + "Trigger deployment to dev env"
  ```

  This applies to branch names too.
  ```diff
  - "rebasing-was-too-hard-so-this-is-new-cluster-branch" <-- real branch name from a teammate
  + "feature/bundle-mechanism"
  + "bugfix/url-typo"
  ```
- ["[git] commit messages should be present tense and
  directive"](https://github.com/git-guides/git-commit#examples-of-git-commit), basically in the form of:
  ```
  This commit will {commit-message}
  This commit will "add new logic to the handle_menu function"
  This commit will "prevent users from passing in negative numbers to the API"
  ```

