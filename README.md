# Pipeline Failure Signatures

This repository contains the failure signature definitions used by the [Pipeline Failure Analyzer](https://github.com/<your-username>/pipeline-failure-analyzer) GitHub Action.

## Usage

Define your failure signatures in `failure-signatures.yml`. See the [Pipeline Failure Analyzer README](https://github.com/<your-username>/pipeline-failure-analyzer#failure-signatures-reference) for the full signature format reference.

## Example

```yaml
- id: 1
  name: "NPM Install Failure"
  description: "npm install failed."
  categories: [build, npm]
  patterns:
    - substring: "npm ERR! code ERESOLVE"
```
