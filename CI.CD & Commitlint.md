# CI/CD
The code for the ci/cd workflow which will call the main CI/CD to check the code qaulity
<!-- 
name: CI

on:
  push:
    branches: [ main ]
  pull_request:

jobs:
  call-ci:
    uses: helbec-tech/.github/.github/workflows/ci.yml@main
    with:
      node-version: "20"
      run-tests: true
      run-lint: true
      build: true
      publish: false
    secrets:
      NPM_TOKEN: ${{ secrets.NPM_TOKEN }}\
-->
The name of the file should be (Workflow/ci.yml)

#COMMITLINT
The code for the commitlint config which will call the main commitlint to check the commits in the repo it was called in.
<!-- 
module.exports = { extends: ['@commitlint/config-conventional'] }; 
-->
