# Google Play Store Data Analytics

An interactive data analytics project exploring Google Play Store applications, ratings, installs, reviews, categories, and user sentiment using Python and Plotly.

> **Project type:** Data Analytics Internship / Training Project  
> **Primary tools:** Python, Pandas, Jupyter Notebook, Plotly, HTML, CSS, JavaScript  
> **Main deliverable:** Interactive HTML dashboard

## Overview

This project analyzes Google Play Store app data to identify patterns in application ratings, installs, reviews, categories, and sentiment. The analysis is developed in a Jupyter Notebook and presented through interactive Plotly visualizations, then assembled into a single HTML dashboard for sharing and display.

The repository includes the consolidated dashboard, the analysis notebook, and a `Tasks/` folder containing individual HTML visualizations created during the project training work.

## Project Structure

```text
├── README.md
├── index.html
├── Google Play Store Analytics.ipynb
├── apps.csv                         # Source dataset; publish only if redistribution is permitted
├── user_reviews.csv                 # Source dataset; publish only if redistribution is permitted
└── Tasks/
    ├── Task 1 - App Size Rating Bubble.html
    ├── Task 2 - Top 5 Category Installs.html
    ├── Task 3 - Monthly Install Trends.html
    ├── Task 4 - Cumulative Installs Area.html
    ├── Task 5 - Top 10 Category Rating Reviews.html
    └── Task 6 - Average Installs Revenue.html
```

*The filenames above reflect the files visible in the screenshots. Keep the actual filenames as they appear on your computer.*

## Project Components

### Main dashboard — `index.html`

The consolidated dashboard brings the task visualizations together in one HTML page. It is designed to display interactive charts and apply time-based visibility windows using Indian Standard Time (IST), as required by the project training workflow.

### Analysis notebook — `Google Play Store Analytics.ipynb`

The notebook contains the Python workflow used to prepare data, apply task-specific filters, aggregate metrics, and create visualizations.

### Training task outputs — `Tasks/`

This folder contains standalone HTML exports for the six project-training tasks. Each file can be opened independently to review its visualization.

## Analytics Tasks

| Task | Analysis | Visualization |
|---|---|---|
| 1 | App size, rating, installs, and review sentiment after applying specified filters | Interactive bubble chart |
| 2 | Installs by category, including top-five category analysis and threshold highlighting | Interactive bar chart |
| 3 | Monthly install trends by category and month-over-month growth | Interactive time-series chart |
| 4 | Cumulative installs over time by category | Interactive area chart |
| 5 | Rating and review comparison for selected top categories | Grouped/dual-axis comparison chart |
| 6 | Average installs and estimated revenue comparison for free and paid apps in selected categories | Dual-axis chart |

**Geographic-data note:** The app dataset shown for this project does not include a country or geographic-location field. Task 2 therefore uses a category-based visualization rather than presenting geographic data.

## Datasets

- **`apps.csv`** — app metadata such as app name, category, rating, review count, size, installs, price, content rating, last-updated date, and Android version.
- **`user_reviews.csv`** — review text, sentiment labels, sentiment polarity, and sentiment subjectivity.

The notebook is the source of truth for the exact transformations and filters applied to each task.

## Data Preparation

Depending on the task, preparation may include:

- Converting install counts and prices from text to numeric values.
- Cleaning app-size and Android-version fields.
- Parsing last-updated dates and deriving monthly periods.
- Handling missing values and excluding records that do not meet task filters.
- Aggregating records by category, month, or app type.
- Calculating growth and estimated revenue metrics.

## Technology Stack

- **Python** — analysis and data preparation
- **Pandas** — data cleaning, filtering, and aggregation
- **Jupyter Notebook** — analysis workflow
- **Plotly** — interactive visualizations
- **HTML, CSS, JavaScript** — dashboard layout and time-based chart visibility

## Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/google-play-store-data-analytics.git
cd google-play-store-data-analytics
```

Replace `<your-username>` with your GitHub username.

### 2. View the dashboard

Open `index.html` in a modern web browser. The generated dashboard is a static HTML page, so the notebook is not required just to view it.

### 3. Run the notebook

Install the main dependencies if they are not already installed:

```bash
python -m pip install pandas plotly jupyter
```

Start Jupyter:

```bash
jupyter notebook
```

Open `Google Play Store Analytics.ipynb` and run the cells in order. Keep the CSV files in the locations expected by the notebook.

## Publish with GitHub Pages

1. Push `index.html` and the files you intend to publish to your GitHub repository.
2. Open **Settings → Pages** in the repository.
3. Under the build/deployment settings, choose **Deploy from a branch**.
4. Select the `main` branch and `/ (root)` folder, then save.
5. Wait for deployment and open the URL displayed in the Pages settings.

Because `index.html` is in the repository root, GitHub Pages can use it as the site entry point. Test the published page after deployment.

## Important Notes

- **Estimated revenue:** If calculated as installs multiplied by listed app price, revenue is only an estimate. Install counts may be approximate, and the calculation does not account for store fees or discounting.
- **No fabricated geography:** Category-level install totals should not be interpreted as country-level data.
- **Time-based visibility:** The dashboard's visibility windows use IST. Verify the published page during each task's intended time window and ensure JavaScript is enabled.
- **Dataset licensing:** Before making the repository public, confirm that you are allowed to redistribute the CSV files. If uncertain, do not upload them; instead, document their source and how they were obtained.
- **Notebook size:** Clear large or unnecessary notebook outputs before committing if they make the repository difficult to browse.

## Future Improvements

- Document dataset sources and licensing.
- Add a data dictionary and methodology section.
- Validate filter and aggregation results automatically.
- Improve accessibility and mobile responsiveness.
- Add dashboard screenshots or a short demo GIF.
- Add the published dashboard link once GitHub Pages is enabled.

## Author

**Sai Deepak**  
B.Tech — Computer Science and Engineering

- GitHub: [Saideepak1806](https://github.com/Saideepak1806)
- LinkedIn: [Sai Deepak](https://www.linkedin.com/in/pindiboina-sai-deepak-341ba7365/)

---

*This project is intended for learning, analytics practice, and portfolio demonstration. Results depend on the supplied datasets and the filters applied in the notebook.*
