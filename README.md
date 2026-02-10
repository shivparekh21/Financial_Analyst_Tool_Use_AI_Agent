# Financial Analyst Tool-Use Agentic AI System

## Overview

An intelligent **Financial Analyst Agentic AI System** designed to assist investors with accurate, up-to-date stock market insights. Built from scratch using **LangGraph**, this system provides comprehensive market analysis and stock-specific insights through dynamic tool usage and intelligent reasoning.

---

## System Architecture

### 1. Agent System Prompt

The core agent is engineered with the following capabilities:

- **Query Validation**: Validates input queries for relevance and specificity
- **Adaptive Analysis**: Provides comprehensive market analysis or stock-specific insights based on query type
- **Professional Guidance**: Responds professionally to invalid queries and guides users appropriately

#### Workflow Flows

**Flow 1: General Market Analysis**
- Analyzes overall market trends
- Suggests stock opportunities based on market data
- Utilizes tools: `SEARCH_WEB`, `GET_GENERAL_MARKET_DATA`

**Flow 2: Stock-Specific Analysis**
- Validates stock ticker symbols
- Retrieves comprehensive stock data
- Provides detailed insights using: `GET_STOCK_FUNDAMENTAL_INDICATOR_METRICS`, `GET_STOCK_PRICE_METRICS`

---

### 2. Financial Analysis Tools

The system integrates multiple specialized tools for comprehensive financial data retrieval:

| Tool | Description |
|------|-------------|
| **SEARCH_WEB** | Fetches general stock market information from the web |
| **GET_STOCK_FUNDAMENTAL_INDICATOR_METRICS** | Provides key financial metrics (P/E ratio, ROE, etc.) |
| **GET_STOCK_NEWS** | Extracts latest news and updates for stocks/markets |
| **GET_GENERAL_MARKET_DATA** | Fetches overall market trends and performance data |
| **GET_STOCK_TICKER** | Validates and retrieves stock ticker symbols |
| **GET_STOCK_PRICE_METRICS** | Retrieves price trends, performance, and metrics |

---

### 3. Stock Market Data Providers

Ensures real-time, reliable data through integration with top-tier providers via **OpenBB**:

- Yahoo Finance
- Finviz
- TMX
- Cboe
- And more...

---

### 4. Message Trimmer

A dedicated component that manages conversation history:

- Trims agent state message history
- Ensures messages remain within LLM context window limits
- Optimizes performance and response quality

---

### 5. Tool-Use Agentic Framework

The system employs **ReAct (Reasoning + Acting)** methodology:

- **Logical Reasoning**: Analyzes queries to understand user intent
- **Dynamic Tool Selection**: Automatically selects appropriate tools based on query requirements
- **Actionable Results**: Combines reasoning with tool execution for precise outcomes

---

### 6. Final Response Generation

After processing data from tool calls, the agentic system:

- Synthesizes information from multiple sources
- Generates comprehensive, actionable insights
- Delivers professional financial analysis tailored to the user's query

---

## Key Features

✅ **Built with LangGraph**: Modern alternative to LangChain for advanced agent orchestration  
✅ **Real-time Data**: Integration with multiple reliable financial data providers  
✅ **Intelligent Reasoning**: ReAct framework for optimal tool selection and usage  
✅ **Context Management**: Automatic message trimming for optimal performance  
✅ **Dual-Mode Analysis**: Supports both general market and stock-specific queries  
✅ **Professional Validation**: Input validation with helpful user guidance  

---

## Use Cases

- **Individual Investors**: Get quick insights on stocks and market trends
- **Financial Analysts**: Automate data gathering and preliminary analysis
- **Portfolio Managers**: Track multiple stocks and market conditions
- **Market Researchers**: Access comprehensive market data and news

---

## Technology Stack

- **Framework**: LangGraph
- **Reasoning Pattern**: ReAct (Reasoning + Acting)
- **Data Platform**: OpenBB
- **Data Sources**: Yahoo Finance, Finviz, TMX, Cboe, and more

## License

*(Add license information here)*
