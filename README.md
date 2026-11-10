# Hi, I'm Cas

I'm a data engineer based in Birmingham. I build warehouse loads, API integrations and data quality tests, and my work runs in production. I also have an MSc in Bioinformatics (Distinction), and I'd like to bring both together in health data.

I'm open to data engineering roles and available immediately.

## Junior Data Engineer, Genting Casinos UK

August to November 2026, Data Warehouse and Integration team. I worked on a PostgreSQL data warehouse for a regulated casino and hotel business, alongside senior engineers and an external solutions architect.

**Built and shipped to production**

- **Rebuilt a third-party training records feed end to end.** Worked out which datasets were needed from a mapping sheet, wrote the PostgreSQL DDL for new dimension and fact tables, and built Pentaho transformations to load scheduled CSV extracts from SFTP. My load replaced the old one, and I then decommissioned the legacy job and raised the network change to cut the old SFTP connection.
- **Built automated file ingestion from SharePoint.** Set up API access through an Azure app registration and used Postman to test Microsoft Graph and SharePoint REST calls, including getting bearer tokens for authentication. Then built the Pentaho jobs and transformations that pull the files through the API and load them, now live.
- **Consolidated spreadsheet data from 32 sites.** Designed the table and built the Pentaho job that loads each site's spreadsheet from SharePoint into one table, mapped site names to warehouse IDs, and worked with the business owner to standardise naming.
- **Built a load template that survives supplier changes.** Used Pentaho metadata injection so columns match by header name rather than position, meaning a load doesn't break when a supplier reorders columns. Pushed to production.
- **Delivered new marketing variables.** Wrote the SQL for a summary table (one row per customer per game type, with days since last played) that the marketing team now use to build targeted customer groups.
- **Prepared a monthly production change to the customer app.** Each month I wrote the change request, the SQL script (from Git templates) and the runbook, and coordinated downtime with the games systems team.

**Running it day to day**

- **Automated data quality testing.** Built a Pentaho transformation that reads the warehouse data dictionary and generates a SQL test for every column, covering 121 testable columns on a customer profile table of over 2 million rows, built to run daily and report results in Tableau.
- **Handled daily job failures.** Picked up failed loads from email alerts, worked out what went wrong and reran them. Rerunning safely means knowing each load's watermark (the marker for how far it got last time), so a rerun doesn't duplicate or skip data.
- **Took changes through the Change Advisory Board.** Attended the board meetings and presented my changes to the other members for approval.
- **Microsoft Fabric migration.** Took part in migration planning, including moving flat-file loads from Pentaho into Fabric.

Company code stays with the company, so none of it is on here. The projects below are my own.

## Tools

- **SQL:** PostgreSQL (CTEs, window functions, DDL, query tuning)
- **ETL:** Pentaho Data Integration (transformations, jobs, metadata injection), SFTP file feeds
- **Cloud and APIs:** Azure app registrations, Microsoft Graph, SharePoint REST, bearer token authentication, Postman, Microsoft Fabric
- **Languages:** Python (pandas, NumPy, scikit-learn, TensorFlow), R, Bash
- **Tools:** DBeaver, Tableau, Git, SLURM (job scheduling on high-performance computing clusters)
- **Ways of working:** change control through a Change Advisory Board, service desk tickets, runbooks, data dictionaries
- **Certification:** Microsoft Fabric Data Engineer Associate, exam booked December 2026

## Before data engineering

**MSc Bioinformatics, University of Birmingham (Distinction).** For my dissertation I built a Python pipeline that turned almost 2,000 cancer mutation files into one table per patient, then checked the output against published figures. That checking caught a gene variant coming back at 0% because the files numbered the gene differently to how I was searching for it. Fixing it recovered 53 patients who had been silently dropped.

**NHS histopathology.** I worked as a lab assistant at the John Radcliffe Hospital, where accurate records and traceability matter for patient safety. It's where I learnt to take data quality seriously.

## Projects

| Project | What it shows |
| --- | --- |
| [Sequential-Clinical-Prediction](https://github.com/CasmirO-Source/Sequential-Clinical-Prediction) | A pipeline that joins three hospital tables, standardises diagnosis codes and turns each admission into a model-ready sequence, plus the model that predicts in-hospital mortality from it |
| [Multiomics-Integration-Pipeline](https://github.com/CasmirO-Source/Multiomics-Integration-Pipeline) | Loading two datasets, handling missing values and joining them on shared sample IDs |
| [COVID-19-Sequence-Tracking](https://github.com/CasmirO-Source/COVID-19-Sequence-Tracking) | Parsing 187 viral genome records and comparing them in plain Python, no libraries |
| [Gene-Identification-Tool](https://github.com/CasmirO-Source/Gene-Identification-Tool) | Calling the NCBI BLAST web service from a script and parsing the XML it sends back |
| [SPIKES](https://github.com/CasmirO-Source/SPIKES) | An app I built as part of a hackathon team (forked from the team repo) |

## Contact

- **Email:** c.t.obi-osuala@outlook.com
- **LinkedIn:** [linkedin.com/in/ctobi](https://www.linkedin.com/in/ctobi)
