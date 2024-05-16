# Customer Experience at Vanguard (A/B Testing)

## Description

This project focuses on enhancing customer experience at Vanguard, a US-based investment management company. The team has launched an exciting digital experiment, and now they are eager to uncover the results. To achieve this, a demographic study was conducted, and two hypotheses were formulated to determine if the new website design was functioning correctly.

## Installation

### Requirements

- **Languages and Tools:**
  - Tableau
  - Python
  
- **Libraries:**
  ```python
  import pandas as pd
  import matplotlib.pyplot as plt
  import seaborn as sns
  import numpy as np
  import scipy.stats as st
  from statsmodels.stats.proportion import proportions_ztest

For more details, please refer to the contents of the `env` folder.

## Configuration

### Data Description

#### Original:

- **df_final_demo:** Contains basic client information.
  
  **Meaning of Variables:**
  - `client_id`: Unique ID of each client.
  - `clnt_tenure_yr`: Represents how long the client has been with Vanguard in years.
  - `clnt_tenure_mnth`: Further breaks down the client’s tenure with Vanguard in months.
  - `clnt_age`: Indicates the age of the client.
  - `gendr`: Specifies the client’s gender.
  - `num_accts`: Denotes the number of accounts the client holds with Vanguard.
  - `bal`: Gives the total balance spread across all accounts for a particular client.
  - `calls_6_mnth`: Records the number of times the client reached out over a call in the past six months.
  - `logons_6_mnth`: Reflects the frequency with which the client logged onto Vanguard’s platform over the last six months.

  **Cleaned as:** `clients`

- **df_final_experiment_clients:** Explains the type of test clients were subjected to.

  **Meaning of Variables:**
  - `client_id`: Unique ID of each client.
  - `variation`: Indicates if a client was part of the experiment.

  **Cleaned as:** `experiment`

#### Experiment:

- **df_final_web_data_pt_1**
- **df_final_web_data_pt_2**

  Describe the experiment.

  **Meaning of Variables:**
  - `client_id`: Unique ID of each client.
  - `visitor_id`: A unique ID for each client-device combination.
  - `visit_id`: A unique ID for each web visit/session.
  - `process_step`: Marks each step in the digital process.
  - `date_time`: Timestamp of each web activity.

  **Cleaned as:** `webs`

### Important

Based on hypothesis formulas for better understanding.

Note: The presentation is structured like a story in the Tableau file.
