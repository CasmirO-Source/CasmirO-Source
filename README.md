# Hi, I'm Cas

I'm a data engineer with an MSc in Bioinformatics (Distinction, University of Birmingham). Most of what I do is taking data from messy sources and turning it into clean, tested tables that people can actually trust. I'm most interested in doing that with health data.

I'm currently open to data engineering roles.

## What I've worked on

**Data engineering.** I've worked as a junior data engineer in a regulated environment. Day to day that meant:

- Building Pentaho jobs to load files from SFTP and spreadsheets into a PostgreSQL warehouse
- Writing SQL test scripts to check new tables against the data dictionary before anything went live
- Building summary tables to feed marketing analytics
- Setting up API access to SharePoint and testing it in Postman before it went through change approval

**MSc dissertation.** I looked at whether eligibility for targeted cancer drugs differs by ethnicity, using over 2,000 patients from The Cancer Genome Atlas (TCGA). A lot of it was data engineering. The clinical data came as 10,365 event-level records, which I collapsed to one row per patient. I parsed almost 2,000 mutation files on a high-performance computing cluster, then checked my outputs against published figures before trusting any result.

That checking paid off. One gene variant was coming back at 0% across the whole dataset because the mutation files numbered that gene differently to how I was searching for it. Fixing it recovered 53 patients who carried the variant and had been silently dropped.

**NHS lab work.** Before the MSc I was a lab assistant in NHS histopathology at the John Radcliffe Hospital, so I've seen first hand where clinical data comes from and how it gets recorded.

## Tools

- **Data:** SQL, PostgreSQL, Trino, Pentaho, SSIS
- **Languages:** Python (pandas, NumPy, scikit-learn, TensorFlow), R, Bash
- **Other:** Git, Postman, SLURM (job scheduling on high-performance computing clusters)
- **Studying for:** Microsoft Fabric Data Engineer certification

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
