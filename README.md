# MCP Design-to-Code Prototype Repository  

This repository provides a skeleton for an agent‑driven design‑to‑code workflow using multiple Model Control Programs (MCPs). It is intended as a starting point for building integrations that convert design artifacts into code while orchestrating tasks between Notion, Figma, and Playwright.  

## Folder Structure  

- `Notion/` – Holds scripts, prompts, and integration stubs for a Notion‑based MCP that extracts design specs or documentation from Notion pages.  
- `Figma/` – Contains code for interacting with Figma via an MCP to retrieve frames or components and transform them into front‑end code.  
- `Playwright/` – Contains a Playwright MCP for automated UI testing and validation of the generated code.  

Each folder currently includes a placeholder README where you can start developing the respective MCP integration.  

## Prompts  

Define clear prompts that instruct each MCP on its responsibilities: retrieving relevant content from Notion, converting Figma designs to code components, and running end‑to‑end tests with Playwright. Prompts can be stored alongside the scripts in the respective folders.  

## Scripts  

Use this repository to organize scripts that automate the design‑to‑code pipeline. Example scripts might:  

- Fetch design specifications from Notion.  
- Use the Figma API to download frames and generate code stubs.  
- Run Playwright tests to verify UI against the design.  

These scripts can live in their respective integration folders or in a `scripts/` directory if shared across MCPs.  

## Continuous Integration  

Set up a basic CI pipeline (for example using GitHub Actions) to run automated tasks on every push. Typical steps might include:  

- Installing dependencies.  
- Running any code generation scripts.  
- Executing Playwright tests.  

A placeholder workflow file (`.github/workflows/ci.yml`) can be added later to define these steps.
