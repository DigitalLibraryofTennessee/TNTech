# TNTech
Data and Transform from Tennessee Tech for initial DPLA ingest in September 2021

Because Preservica's OAI-PMH service was not accessible, we decided to simply transform a CSV from TN Tech into MODS.

## Repository Structure

```
|-- cleaned_data
    |-- tntech21.xml
    |-- remediation_files
        |-- TennTech2021Ingest.openrefine.tar.gz
        |-- tntech21.xpr
        |-- tntechMODS.xml
	      |-- open_refine_template.md
        |-- clean.xsl
|-- original_data
    |-- TTU2021Septingest.csv
