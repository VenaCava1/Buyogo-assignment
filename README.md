# Buyogo-assignment
Assignment for Buyogo Internship

# Hotel Booking Analytics & QA System

## Overview
This system provides analytics and question-answering capabilities for hotel booking data using LLM-powered RAG.

## Features
- Revenue trend analysis
- Cancellation rate tracking
- Geographical distribution visualization
- Natural language question answering
- REST API endpoints

## Setup
1. Clone the repository
2. Install requirements: `pip install -r requirements.txt`
3. Download the dataset (or use provided sample)
4. Run data processing: `python data_processing.py`
5. Start API: `uvicorn main:app --reload`

## API Endpoints
- `POST /analytics` - Get precomputed analytics
- `POST /ask` - Ask natural language questions

## Examples
See `sample_queries.json` for test queries and expected responses.
