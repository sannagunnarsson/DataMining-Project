# Data Mining I Project

## Social Interaction Patterns and Phone Call Responsiveness Among University Students

This repository contains the code and analysis for our Data Mining I project.

The project investigates whether patterns in previous interactions between two university students are associated with whether a phone call between them is answered or missed.

## Research Question

**What patterns in previous interactions between two university students are associated with whether a phone call between them is answered or missed?**

The aim is to identify recurring combinations of previous interaction behaviour related to answered and missed calls.

## Dataset

We use data from the **Copenhagen Networks Study**, which contains interaction data from more than 700 university students.

The available data includes:

- Phone calls
- SMS messages
- Bluetooth proximity
- Facebook friendships
- Gender information

The main dataset used in the project is the phone call data.

For each phone call, only information from interactions that occurred **before the call** will be used.

Dataset source:
Copenhagen Networks Study  
https://figshare.com/articles/dataset/The_Copenhagen_Networks_Study_interaction_data/7267433/1

## Planned Analysis

The project includes:

### Exploratory Data Analysis

Initial analysis of:

- Number of calls
- Answered vs missed calls
- Call duration
- Calls over time
- Interaction frequency
- Missing values
- Potential incorrect or unusual values

### Preprocessing

Features may include:

- Number of previous calls between two participants
- Proportion of previous calls that were answered
- Time since previous call
- Number of recent SMS messages
- Time since previous SMS
- Recent Bluetooth proximity
- Previous answering rate of the receiver
- Time of day
- Day of week
- Weekday or weekend

Continuous variables may be discretized when needed.

### Data Mining Methods

The main methods considered are:

- Association Rule Mining
- Clustering

Association Rule Mining will be used to identify combinations of interaction characteristics associated with answered or missed calls.

Clustering may be used to identify groups with similar interaction profiles.

## Project Structure

```text
DataMining/
│
├── README.md
├── .gitignore
│
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_preprocessing.ipynb
│   ├── 03_association_rules.ipynb
│   └── 04_clustering.ipynb
│
├── src/
│   └── preprocessing.py
│
└── data/
    ├── calls.csv
    ├── sms.csv
    ├── bt_symmetric.csv
    ├── fb_friends.csv
    └── genders.csv
