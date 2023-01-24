# mult-br


name: Status Check
on: [pull_request]

 

jobs:
  test-and-lint:
    runs-on: ubuntu-latest
    steps:
    - name: Checkout code
    uses: actions/checkout@v2

 

    - name: Run tests
    run: npm test

 

    - name: Lint code
    run: npm run lint
