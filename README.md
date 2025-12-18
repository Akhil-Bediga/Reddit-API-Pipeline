Architecture
------------------------
<img width="580" height="267" alt="Architecture" src="https://github.com/user-attachments/assets/5277d77c-1553-403c-b04c-54dd301f2996" />


1. Extract data using Reddit API
2. Load into AWS S3
3. Copy into AWS Redshift
4. Transform using dbt
5. Create PowerBI or Google Data Studio Dashboard
6. Orchestrate with Airflow in Docker
7. Create AWS resources with Terraform

Output
------------
<img width="580" height="391" alt="Output" src="https://github.com/user-attachments/assets/f90a72b5-dc3e-45aa-9e6f-d9344e022297" />
* Final output from Google Data Studio.
* Note that Dashboard is reading from a static CSV output from Redshift. Redshift database was deleted so as not to incur cost.

Setup
-----
Follow below steps to setup pipeline. I've tried to explain steps where I can. Feel free to make improvements/changes.
>**note**: This was developed using an M3 pro Macbook Pro. If you're on Windows or Linux, you may need to amend certain components if issues are encountered.

As AWS offer a free tier, this shouldn't cost you anything unless you amend the pipeline to extract large amounts of data, or keep infrastructure running for 2+ months. However, please check AWS free tier limits, as this may change.

First clone the repository into your home directory and follow the steps.

```bash
[git clone https://github.com/Akhil-Bediga/Reddit-API-Pipeline.git
cd Reddit-API-Pipeline
```

1. [Overview](instructions/overview.md)
1. [Reddit API Configuration](instructions/reddit.md)
1. [AWS Account](instructions/aws.md)
1. [Infrastructure with Terraform](instructions/setup_infrastructure.md)
1. [Configuration Details](instructions/config.md)
1. [Docker & Airflow](instructions/docker_airflow.md) 
1. [dbt](instructions/dbt.md)
1. [Dashboard](instructions/visualisation.md)
1. [Final Notes & Termination](instructions/terminate.md)
1. [Improvements](instructions/improvements.md)
