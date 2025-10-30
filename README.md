SOC Brute-Force Detection & Analysis — Colab Simulation

Author: Utkarsh Walchale

Purpose: This repository contains a simple, interview-ready SOC simulation implemented in Python (suitable for Google Colab or local Jupyter). The lab simulates SSH login logs, detects brute-force activity, enriches suspicious IPs with geolocation data, visualizes results, and automatically classifies incident severity. It’s designed to demonstrate practical SOC skills you can discuss in interviews.

Table of Contents

-1 Overview

-2 Use Cases

-3 Prerequisites

-4 Files

-5 How to run (Colab)




1. Overview

This simulation reproduces a SOC-style workflow for detecting SSH brute-force attacks from log data. The pipeline includes:

Synthetic log generation (failures and successes)

Detection of suspicious IP addresses (based on failed login counts)

Identification of potential compromises (success after failures)

Geolocation enrichment (country, city, organization)

Visualization of attacks

Severity scoring and classification

Auto-generated SOC-style summary and recommended actions

All steps are implemented in plain Python using pandas and matplotlib, and the script uses ip-api.com for simple geolocation lookups.


2. Use Cases

Interview demo: show your ability to perform detection, enrichment and triage.

SOC training: quick way to simulate alerts and practice triage logic.

Demo for automation: illustrate how basic rules & enrichment create prioritized alerts.


3. Prerequisites

Python 3.8+ (Colab already has Python installed)

Packages: pandas, matplotlib, requests

(Optional) VirusTotal API key if you want to enrich with threat intelligence.

Install missing packages locally with:

pip install pandas matplotlib requests


4. Files

This README contains a single-file Python script that you can paste into a Colab cell or a Jupyter notebook. Optionally, you can split the sections into separate cells for interactive use.


5. How to run (Colab)

Open https://colab.research.google.com

Create a new notebook

Copy the full script from the "Full script" section below into a cell

Run the cell

(Optional) Download the notebook as PDF: File -> Download -> PDF to attach to interviews or portfolios
