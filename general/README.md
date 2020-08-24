# General Guidelines

Style and best practices that apply to all languages and frameworks.

- These are not to be blindly followed; strive to understand these and ask when
  in doubt.
- Don't duplicate the functionality of a built-in library.
- Don't swallow exceptions or "fail silently."
- Don't write code that guesses at future functionality.
- Exceptions should be exceptional.
- Keep the code simple.

## Formatting

- Avoid inline comments.
- Break long lines after 80 characters.
- Delete trailing whitespace.
- Use empty lines around multi-line blocks.
- Use spaces around operators, except for unary operators, such as `!`.
- Use [uppercase for SQL key words and lowercase for SQL identifiers].


## Naming

- Avoid abbreviations.
- Prefer naming classes after domain concepts rather than patterns they
  implement.
- Name the enumeration parameter the singular of the collection.
- Name variables, methods, and classes to reveal intent.

## Organization

- Order methods so that caller methods are earlier in the file than the methods
  they call.
- Order methods so that methods are as close as possible to other methods they
  call.
