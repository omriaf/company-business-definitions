# Company business definitions

This repository is the governed business-logic source for the company analytics
routing agent. Each YAML file under `definitions/` owns one metric: its plain-language
meaning, domain, approved resolution target, and proxy status.

Edit and merge a definition here; the Databricks App polls the latest `definitions/`
commit and adopts the validated snapshot without a redeploy. Invalid or undefined terms
fail loud rather than being guessed.
