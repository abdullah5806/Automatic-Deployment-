# SOM Lab: CI/CD Pipeline Deployment

This repository contains a simple static website used to demonstrate Continuous Integration and Continuous Deployment (CI/CD) using GitHub Actions.

## 🔗 Live Deployed Website

<!-- **[INSERT YOUR GITHUB PAGES URL HERE]** -->

https://abdullah5806.github.io/Automatic-Deployment-/

## ⚙️ Pipeline Steps

This project utilizes GitHub Actions as the CI/CD tool. The workflow (`deploy.yml`) consists of the following automated steps:

1. **Trigger:** The pipeline is triggered automatically on every `push` to the `main` branch.
2. **Checkout:** The pipeline spins up an `ubuntu-latest` virtual server and uses the `actions/checkout@v4` action to pull down the latest code from the repository.
3. **Setup & Upload:** It configures GitHub Pages and packages the static HTML/CSS files into a deployable artifact.
4. **Deploy:** The `actions/deploy-pages@v4` action pushes the artifact to GitHub's hosting servers, making the website live.

## 🚀 Deployment Process

The deployment process is entirely fully automated.

1. A developer writes or updates code locally on their machine.
2. The developer commits the changes and pushes them to the `main` branch on GitHub.
3. GitHub Actions immediately detects the push and runs the pipeline.
4. Within minutes, the live website is updated without any manual server configuration or FTP file transfers.