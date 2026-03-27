# Music ETL & Analysis Project

A data engineering project examining the evolution of music audio features over time and the influence of TikTok on song popularity and chart performance.

## Description

This project investigates how song characteristics such as loudness, duration, danceability, energy, tempo, key, mode, and time signature have changed historically, and how TikTok has shaped modern music trends. Using historical Spotify data (1960–2015) alongside TikTok viral songs and Spotify Top Charts data (2019–2022), the project implements an ETL pipeline with Python, pandas, MySQL, and Apache Airflow, containerized with Docker. Visualizations and dashboards are created using Plotly and Dash, enabling exploration of trends such as the "Loudness War," increases in energy and danceability, and the chart longevity of TikTok-trending tracks.

## Getting Started

### Dependencies

- Python 3.9+
- pandas, SQLAlchemy
- MySQL
- Apache Airflow
- Docker & Docker Compose
- Plotly, Dash

### Installing

1. Clone the repository:
```bash
   git clone https://github.com/JoshuaE43/dev10-capstone.git
```
2. Ensure MySQL is running and accessible within Docker containers.
3. Primary dataset too large for GitHub. Download from Kaggle and place in datasets/primary/.
https://www.kaggle.com/datasets/rodolfofigueroa/spotify-12m-songs



### Executing

1. Build and start Docker containers:
```bash
   docker-compose up --build
```
2. Access Airflow at `http://localhost:8080` and trigger the `music_etl_dag`.
3. Load datasets via mounted volumes or update paths in configuration files.
4. Launch the Dash app:
```bash
   python dash_app/app.py
```

## Help

For common issues with Airflow or Docker:
```bash
docker-compose logs
docker-compose down --volumes --remove-orphans
```
Check dataset paths and column names if errors occur during ETL.

## Authors

Joshua Eapen — [@JoshuaE43](https://github.com/JoshuaE43)

## Version History

- **0.2** — Refactored ETL into `ETLProcessor` class, added Airflow DAG, Docker, and Plotly/Dash visualizations
- **0.1** — Initial release, basic CSV ingestion and MySQL loading

## License

This project is licensed under the [MIT License](LICENSE.md).

## Acknowledgments

- Figueroa, R. (n.d.). *Spotify 1.2M+ songs* [Data set]. Kaggle. https://www.kaggle.com/datasets/rodolfofigueroa/spotify-12m-songs
- Sveta151. (2022). *TikTok impact on the top charts* [Source code]. GitHub. https://github.com/Sveta151/TikTok_impact_on_the_top_charts