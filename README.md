# AI-Powered Weather Agent with n8n Workflows

## Introduction

This project implements an AI-powered weather agent using **n8n**, an automation tool that integrates multiple services seamlessly. The agent fetches real-time weather data from **OpenWeatherMap** and utilizes an **AI-driven Groq Chat Model** to generate intelligent, contextual responses.

## Features

- **Automated Weather Updates**: Retrieves real-time weather data.
- **AI-Powered Responses**: Uses an **LLM-based chat model** to process user queries intelligently.
- **Memory Buffer Support**: Maintains conversation context.
- **Seamless Integrations**: Connects with Wikipedia, n8n workflows, and other APIs for enriched responses.
- **Expandable Workflow**: Can be enhanced with additional services.

---

## Workflow Overview

### 1️⃣ Receiving User Input

- The workflow starts when a user sends a weather-related query.
- The **Groq Chat Model** processes the message.
- The **memory buffer** ensures context retention.
- The workflow can fetch additional information from **Wikipedia** or other connected APIs.

### 2️⃣ Processing Weather Data

- The workflow queries **OpenWeatherMap** for the latest weather conditions.
- The retrieved data is passed through a **Basic LLM Chain** for contextual interpretation.
- The AI analyzes and structures the weather data meaningfully.

### 3️⃣ Finalizing the Response

- A second **LLM chain** refines the processed weather information.
- The final response is formatted to be clear, concise, and user-friendly.
- The formatted message is sent back to the user via the chat interface.

---

## Tech Stack

| Component         | Description |
|------------------|-------------|
| **n8n**         | Low-code automation tool for workflow orchestration |
| **OpenWeatherMap** | API providing real-time weather data |
| **Groq Chat Model** | AI-powered model for intelligent responses |
| **LLM Chains**  | Used for processing and refining responses |
| **Memory Buffer** | Maintains conversation context |

---

## Installation & Setup

### Prerequisites

- **n8n** installed on your system ([Installation Guide](https://docs.n8n.io/))
- OpenWeatherMap API key ([Get API Key](https://openweathermap.org/api))
- Basic knowledge of n8n workflow automation

### Steps to Set Up

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-repo/ai-weather-agent.git
   cd ai-weather-agent
