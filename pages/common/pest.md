# pest

> A PHP testing framework with a focus on simplicity.
> More information: <https://pestphp.com>.

- Initialize a standard Pest configuration in the current directory:

`pest --init`

- Run tests in the current directory:

`pest`

- Run tests annotated with the given group:

`pest --group {{name}}`

- Run tests and print the coverage report to `stdout`:

`pest --coverage`

- Run tests with coverage and fail if the coverage is less than the minimum percentage:

`pest --coverage --min={{80}}`

- Run tests in parallel:

`pest --parallel`

- Run tests with mutations:

`pest --mutate`
