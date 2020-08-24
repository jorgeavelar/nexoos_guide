# Testing with RSpec

- Avoid the `private` keyword in specs.
- Separate setup, exercise, verification, and teardown phases with newlines.
- Use RSpec's [`expect` syntax].
- Use RSpec's [`allow` syntax] for method stubs.
- Avoid using instance variables in tests.
- Disable real HTTP requests to external services with `WebMock.disable_net_connect!`.
- Don't test private methods.
- Test background jobs with a [`Delayed::Job` matcher].
- Use a single level of abstraction within scenarios.
