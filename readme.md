# Regional- und Stadtökonomik Analysis

This repository contains code and data for the analysis of regional and urban economics literature, focusing on metrics and methods used in published papers.

## Structure

- `analysis.ipynb`: Main Jupyter notebook containing all code for data processing, clustering, and analysis.
- `dictionaries/metrics.yml`, `dictionaries/methods.yml`: YAML files defining clustered metrics and methods, including synonyms and categories.
- `papers.yml`: Raw papers data.
- `cleared_papers.yml`: Output file with papers annotated by metric/method categories.
- `plots/`: Directory for generated visualizations (bar charts, heatmaps, network graphs, etc.).
- `.gitignore`: Ignores virtual environment files.
- `requirements.txt`: Python dependencies.

## Main Features

- **Pre-processing**: Extracts and checks metrics/methods from papers, compares with YAML dictionaries, and identifies missing items.
- **Clustering**: Assigns metrics and methods from papers to defined categories using synonyms and names.
- **Analysis**: 
  - Counts and visualizes frequency of metrics/methods.
  - Generates co-occurrence heatmaps for categories.
  - Creates timeline and scatter plots for metric usage over time.
  - Builds and visualizes paper networks based on shared metrics/methods.
  - Produces a systematic review table summarizing papers, authors, categories, and timespans.

## Usage

1. **Install dependencies**:
   ```
   pip install -r requirements.txt
   ```

2. **Run the notebook**:
   - Open `analysis.ipynb` in Jupyter.
   - Execute cells in order to process data, cluster items, and generate analyses/plots.

3. **Outputs**:
   - Updated papers with categories: `cleared_papers.yml`
   - Visualizations: saved in `plots/`
   - Review table: printed in notebook, optionally exportable to CSV.

## Customization

- Update `dictionaries/metrics.yml` and `dictionaries/methods.yml` to refine clusters and synonyms.
- Add new papers to `papers.yml` and rerun the notebook for updated analysis.

