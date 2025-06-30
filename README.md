# Azure Feedback Analyzer Logic App

This project contains an Azure Logic App that analyzes customer feedback using Azure Cognitive Services Text Analytics API. It processes blob storage files, detects sentiment, and helps you understand customer emotions.

## Features

- Trigger when a new blob is added or modified in Azure Blob Storage.
- Calls Azure Text Analytics API to detect sentiment in the feedback.
- Parses and processes sentiment scores.
- Ready for CI/CD deployment using ARM templates.

## Project Structure

azure-feedback-analyzer/infra/logicapp/template.json parameters.json 


## Prerequisites

- Azure subscription with Azure Blob Storage and Cognitive Services (Text Analytics) set up.
- Azure CLI or Azure Portal access to deploy the Logic App.
- Git installed for version control.
- GitHub account (optional for CI/CD integration).

## How to Deploy

1. Edit `parameters.json` with your Azure resource details.
2. Use Azure CLI or Portal to deploy the ARM template (`template.json`).
3. Set up your Azure Blob Storage container and upload feedback files.
4. Logic App triggers automatically and processes feedback sentiment.

## Using GitHub

- You can push this project to your GitHub repo to enable CI/CD automation.
- Use GitHub Actions or Azure DevOps pipelines for automated deployments.

## Notes

- Make sure your Cognitive Services subscription key and endpoint are valid.
- Blob container names must be lowercase and match what’s configured in the Logic App.
- The Logic App uses JSON schema to parse the Text Analytics API response.

