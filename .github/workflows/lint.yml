name: lint

on:
  push:
    branches: [ master ]
  pull_request:
    branches: [ master ]

jobs:
  build:
    name: lint
    runs-on: ubuntu-latest
    steps:
      - name: Checkout code
        uses: actions/checkout@v2
      - name: Lint code
        uses: github/super-linter@v4
        env:
          VALIDATE_ALL_CODEBASE: true
          DEFAULT_BRANCH: master
          VALIDATE_BASH: true
          VALIDATE_MARKDOWN: true
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
