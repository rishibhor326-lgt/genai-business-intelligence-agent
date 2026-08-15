# GenAI Business Intelligence Agent

A Generative AI-powered Business Intelligence agent built using Python, Google ADK, Gemini, BigQuery, and the BigQuery MCP Server.

## Project Overview

This project demonstrates how an AI agent can help users interact with data using natural language instead of manually writing SQL queries.

The agent receives a user's question, understands the request, uses the BigQuery MCP Server to interact with BigQuery, retrieves relevant data, and provides a business-oriented response.

This project was developed as part of the Google Cloud Gen AI Academy – Cohort 3.

## Problem Statement

Business users often need data insights but may not always know how to write SQL queries or directly interact with cloud data warehouses.

This project explores how Generative AI and AI agents can make data analysis more accessible by allowing users to ask questions about data using natural language.

## Objective

The objective of this project is to build an AI-powered Business Intelligence assistant that can:

- Understand natural-language questions
- Identify relevant information from a BigQuery dataset
- Generate appropriate SQL queries
- Retrieve data through the BigQuery MCP Server
- Analyze the retrieved information
- Provide useful business-oriented responses

## Technologies Used

- Python
- Google ADK (Agent Development Kit)
- Gemini
- BigQuery
- BigQuery MCP Server
- Model Context Protocol (MCP)
- Google Cloud

## Dataset

This project uses the public New York City Citi Bike dataset available through Google BigQuery:

`bigquery-public-data.new_york_citibike`

The dataset contains information related to Citi Bike trips and can be used to explore questions around bike usage, trip patterns, stations, and other data-driven insights.

## How the Agent Works

The agent follows a simple workflow:

1. The user asks a question in natural language.
2. The AI agent interprets the user's request.
3. The agent determines what information is required from the dataset.
4. The agent uses the BigQuery MCP Server to interact with BigQuery.
5. A SQL query is executed in read-only mode.
6. The retrieved data is provided back to the agent.
7. The agent analyzes the information.
8. The agent provides the result in a natural-language response.

## Architecture

```text
User
  ↓
Natural-Language Question
  ↓
Gemini-powered AI Agent
  ↓
Google ADK
  ↓
BigQuery MCP Server
  ↓
Google BigQuery
  ↓
Citi Bike Dataset
  ↓
Data Retrieved
  ↓
AI Agent Analysis
  ↓
Business-oriented Response
