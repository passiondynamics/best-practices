## Python

### Style
- Use a linter to *mostly* standardize style differences (`black` is what we currently use).
- We usually use 4 spaces to indent.

### Documentation
- pydocs (comments at the top of each function with details about it) are really helpful as we build out our codebases,
  e.g.
  ```python
  def hello(name: str) -> int:
      """
      Print out a welcome message to the user.

      :param: name - the name of the user we're saying hello to.
      :return: a random number that the author of this function really likes!
      """

      print(f"Hello {name}!")
      return -1
  ```
- Python, in later versions, supports type hinting for function parameters. While they're not enforced by the compiler
  *at all*, they're usually picked up by the IDE you're using and warns you if it doesn't match (think VSCode does it
  for example). The example above has some + more complex hints can be built via the `typing` built-in package:
  ```python
  from typing import Dict, List

  def hello2(names: List[str]) -> Dict[str, int]:
      """
      Print out welcome messages for each user given.

      :param: names - a list of user names.
      :return: a map of the authors of this function to their favorite numbers!
      """

      for n in names:
          print(f"Hello {n}!")

      return {"irith": 8}
  ```
