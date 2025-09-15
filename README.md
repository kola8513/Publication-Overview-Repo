# Publication-Overview-Repo

Ein Repository zur Zusammenfassung und Analyse wissenschaftlicher Publikationen – einschließlich Beispieldaten, Skript und Visualisierung mit R und RMarkdown.  
Ideal, um einen Überblick über Ihre Publikationen im Laufe der Jahre und mit verschiedenen Affiliations zu demonstrieren.

## 📈 Funktionen

- **Publikationsdaten:** Beispieldateien im CSV-Format mit Metadaten zu Publikationen (Titel, Autoren, Jahr, Zugehörigkeit etc.)
- **Analyse-Skripte:** R- und RMarkdown-Skripte zur Zusammenfassung und Visualisierung von Publikationstrends.
- **Übersichts-Plot:** Balkendiagramme nach Jahr und Autorenschaftskategorie.
- **Einfache Reproduzierbarkeit:** Alle Daten und Codes sind enthalten und ermöglichen die einfache Wiederholung der Analyse.

## 🗂 Verzeichnisstruktur

```
├── data/
│   └── Example_Publications.csv
├── scripts/
│   └── publication_summary.Rmd
├── plots/
│   └── publication_summary.pdf
├── README.md
```

## 🚀 Schnellstart

1. **Repository klonen**  
   `git clone https://github.com/<Ihr-Benutzername>/publication-overview-repo.git`

2. **Publikationsdaten hinzufügen**  
   Eigene CSV-Datei im `data/`-Ordner ablegen.

3. **Analyse ausführen**  
   Öffnen Sie `scripts/publication_summary.Rmd` in RStudio und führen Sie das Skript aus (Knit zu PDF/HTML).

## 🛠 Voraussetzungen

- R (>= 4.0.0)
- R-Pakete: `ggplot2`, `dplyr`, `forcats`, `ggpubr`, `readr`, `tidyverse`

Installation in R:
```r
install.packages(c("ggplot2", "dplyr", "forcats", "ggpubr", "readr", "tidyverse"))
```

## 💡 Anpassung

- Ersetzen Sie `Example_Publications.csv` durch Ihre eigenen Publikationsdaten.
- Bearbeiten Sie das Skript `publication_summary.Rmd` nach Ihren Wünschen.

## 📚 Lizenz

Dieses Repository steht unter der MIT-Lizenz.

---

## Scroll down for English

---

# Publication-Overview-Repo

A repository to showcase a summary and analysis of academic publications, including example data, script, and plot using R and RMarkdown.  
Ideal for demonstrating your publication overview over the years with different affiliations.

## 📈 Features

- **Publication Data:** Example CSV files with metadata about publications (title, authors, year, affiliation, etc.)
- **Analysis Scripts:** R and RMarkdown scripts for summarizing and visualizing publication trends.
- **Overview Plot:** Bar plots by year and authorship category.
- **Easy Reproducibility:** All data and code included for seamless analysis reproduction.

## 🗂 Repository Structure

```
├── data/
│   └── Example_Publications.csv
├── scripts/
│   └── publication_summary.Rmd
├── plots/
│   └── publication_summary.pdf
├── README.md
```

## 🚀 Getting Started

1. **Clone the repository**  
   `git clone https://github.com/<your-username>/publication-overview-repo.git`

2. **Add your publication data**  
   Place your own CSV file in the `data/` folder.

3. **Run the analysis**  
   Open `scripts/publication_summary.Rmd` in RStudio and Knit to PDF/HTML to generate the plot.

## 🛠 Requirements

- R (>= 4.0.0)
- R packages: `ggplot2`, `dplyr`, `forcats`, `ggpubr`, `readr`, `tidyverse`

Install in R:
```r
install.packages(c("ggplot2", "dplyr", "forcats", "ggpubr", "readr", "tidyverse"))
```

## 💡 Customization

- Replace `Example_Publications.csv` with your own publication data.
- Edit `publication_summary.Rmd` to adjust the analysis and visualization.

## 📚 License

This repository is licensed under the MIT License.
