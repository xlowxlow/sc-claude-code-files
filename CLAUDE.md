# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This repository contains educational materials and practical examples from the "Claude Code: A Highly Agentic Coding Assistant" short course. It includes reading notes, data analysis examples, and references to external RAG chatbot and dashboard projects.

## Development Commands

### Python Environment Setup
```bash
# Install dependencies for the ecommerce data analysis project
pip install -r lesson7_files/requirements.txt
```

### Running Applications

**Streamlit Dashboard**:
```bash
# Run the ecommerce analytics dashboard
streamlit run lesson7_files/dashboard.py
```

**Jupyter Notebooks**:
```bash
# Start Jupyter for data analysis notebooks
jupyter notebook lesson7_files/EDA_Refactored.ipynb
```

## Architecture & Code Organization

### Main Components

1. **Course Materials** (`/reading_notes/`, `/updated_reading_notes/`)
   - Lesson notes with prompts and feature implementations
   - Best practices and workflow examples

2. **Ecommerce Analytics System** (`/lesson7_files/`)
   - **Data Layer** (`data_loader.py`): Handles CSV data ingestion and processing for orders, products, customers, reviews, and payments datasets
   - **Business Logic** (`business_metrics.py`): Calculates KPIs including revenue metrics, product performance, geographic analysis, and customer satisfaction
   - **Presentation Layer** (`dashboard.py`): Streamlit-based interactive dashboard with real-time filtering and Plotly visualizations
   - **Analysis** (`EDA_Refactored.ipynb`): Configurable Jupyter notebook for detailed business analysis

### Key Design Patterns

- **Modular Architecture**: Separation of data loading, metrics calculation, and visualization into distinct modules
- **Configurable Analysis**: Year and month filters can be set as parameters without code changes
- **Reusable Components**: `BusinessMetricsCalculator` and `MetricsVisualizer` classes for consistent metric generation across notebook and dashboard

### Data Flow

1. Raw CSV files → `EcommerceDataLoader` → Processed DataFrames
2. Processed data → `BusinessMetricsCalculator` → Business metrics and reports
3. Metrics → Dashboard/Notebook → Interactive visualizations and insights

## External Project References

The course includes work with these external repositories:
- **RAG Chatbot**: https://github.com/https-deeplearning-ai/starting-ragchatbot-codebase.git (Lessons 2-6)
- **FRED Dashboard**: https://github.com/https-deeplearning-ai/FRED-dashboard.git (Lesson 8)