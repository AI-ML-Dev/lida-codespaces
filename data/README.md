# Data Descriptions

This document will be used to describe the datasets available in this directory, with links to relevant sources or provenance for reproducibility.

---

##  1. Dataset: `atlantis.csv`

This is the default dataset provided by the the [Github codespace-jupyter](https://github.com/github/codespaces-jupyter) template. It contains a simple set of data records with 2 columns (`year`,`population`) that can be used with the `notebooks/population.ipynb` Notebook example for visualization.


## 2. Dataset: `learn-catalog.csv`

This is a dataset obtained using the [Microsoft Learn Catalog API](https://learn.microsoft.com/en-us/training/support/catalog-api#how-the-learn-catalog-api-works) - a REST-based API that returns a JSON-encoded result by default. Currently, there's no authentication required to access the Microsoft Learn Catalog API - and the team has provided [guidance](https://learn.microsoft.com/en-us/training/support/catalog-api-get-started-curl-vscode) to help anyone get started exploring the data for their own projects.

I followed [these guidelines to export the JSON into a flatfile CSV format](https://learn.microsoft.com/en-us/training/support/catalog-api-get-started-curl-vscode#convert-the-response-to-a-spreadsheet) that we can now use for visual exploration with LIDA.

```bash
# First, grab the catalog data in the default JSON format
# This is a 14M download and takes a few seconds to download.  
$ curl https:/learn.microsoft.com/api/catalog >> mslearn-catalog-oct-2023.json

# Follow guidelines above by visiting https://csvjson.com/json2csv
# Upload the json file, then click convert to get flatfile CSV format
# Download the file, rename it to mslearn-catalog-oct-2023.csv
```

You can find the relevant CSV file under `data/mslearn-catatlog-oct-2023.csv`
