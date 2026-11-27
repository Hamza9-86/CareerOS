# CareerOS — System Architecture

## 1. Purpose

CareerOS is a full-stack job search management and job-market intelligence platform. It allows users to manage applications, discover opportunities, analyze market trends, and track job-search performance.

## 2. System Components

### Frontend
React and TypeScript application responsible for UI, user interaction, state, and communicating with the backend API.

### Backend
Node.js and Express API responsible for business logic, validation, authentication, and database operations.

### Operational Database
MongoDB stores users, job postings, saved jobs, applications, and activity records.

### Data Engineering
Python pipelines ingest job postings, preserve raw records, clean and standardize data, deduplicate postings, and generate analytical datasets.

### Analytics
DuckDB and SQL process Parquet datasets to generate job-market insights and application metrics.

## 3. Data Flow

1. Job data is collected from permitted sources.
2. Raw records are stored in the Bronze layer.
3. Data is cleaned, standardized, and deduplicated in the Silver layer.
4. Analytics-ready datasets are generated in the Gold layer.
5. CareerOS consumes analytical results for insights and dashboards.

## 4. Technology Stack

- React
- TypeScript
- Node.js
- Express
- MongoDB
- Python
- Parquet
- DuckDB
- SQL
- Docker
- GitHub Actions

## 5. Architectural Principles

- Separation of concerns
- Modular design
- Data validation
- Secure configuration
- Reproducible processing
- Testability
- Incremental development