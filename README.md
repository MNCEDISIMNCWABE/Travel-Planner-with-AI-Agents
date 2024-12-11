# AI-Powered Travel Planner using CrewAI Agents

## What are AI Agents
AI agents are autonomous systems that perform specific tasks by interacting with tools, data, or users. They leverage AI models to analyze input, make decisions, and produce useful results without constant human supervision.

### General Description:
An AI agent typically has:
- A defined goal: The specific task it is designed to complete.
- Tools or resources: Systems it interacts with, like APIs, databases, or search engines.
- A decision-making process: Often powered by AI models, enabling the agent to adapt to varying situations.

Example:
Imagine you want to bake a cake but don't know how to get started. An AI agent designed for this task could:
- Search for recipes online: Gather information from cooking websites.
- Create a shopping list: Identify ingredients needed and suggest nearby stores to buy them.
- Guide the baking process: Provide step-by-step instructions as you prepare the cake.
The AI agent simplifies the process, saves you time just like a virtual assistant helping with a real-life goal.

This repository demonstrates how to use AI agents to create a comprehensive and personalized travel plan, including flight options, accommodations, activities, and itineraries. By leveraging LangChain, CrewAI and Streamlit for front end, you can simplify travel planning in a dynamic and interactive way. In this repo, I used CrewAI as the primary framework because it enables the integration of tools with virtually any open-source LLM.

To learn more about CrewAI Agents, please visit [CrewAI](https://docs.crewai.com/introduction).

## Setup

### Prerequisites

- LLM Server: This server is responsible for running inferences using the selected language model (LLM). It can operate as a remote server, such as OpenAI’s service, or as a locally hosted instance.
- Install [Ollama](https://ollama.com/) to run LLMs locally. Alternatively, you can use any local LLM server such as[ LM Studio](https://lmstudio.ai/), but this project specifically uses Ollama.
- Create an account with [Serper API ](https://serper.dev/) to obtain an API key for internet search functionality, you will get 2500 free searches.

### Install Libraries
- ```pip install streamlit crewai langchain requests```

Run the app:
```
git clone https://github.com/MNCEDISIMNCWABE/Travel-Planner-with-AI-Agents.git
cd Travel-Planner-with-AI-Agents
streamlit run app.py
```

## Features

1. Two AI Agents:

- Travel Research Specialist: Finds relevant information about budget-friendly flights, accommodations, and activities to do at destination from the internet.

- Vacation Itinerary Creator: Crafts a detailed, day-by-day itinerary based on the Travel Research Specialist's agent findings.

2. Dynamic Tasks: Each agent executes specific tasks, like planning the vacation budget and creating the itinerary.

3. Streamlit Interface: User-friendly front-end for inputting trip details and viewing results.

4. Real-Time Internet Search: Integrated with custom tools for fetching relevant data from the internet.

5. Open Source: Easily adaptable for other use cases like business trip planning, event organization, etc.

## How It Works

1. Input: Provide your travel details, such as departure location, destination, number of travelers, and trip duration (days).

2. AI Collaboration:

- The Travel Planner gathers relevant travel options and estimates costs.
  
- The Vacation Itinerary Creator structures the gathered information into a day-by-day plan.

Output:

- Breakdown of flights, accommodations, and activities.

## Technologies Used

- LangChain: Framework for building AI agents and managing workflows.

- CrewAI: Simplifies multi-agent task execution.

- LLMs (Language Learning Models): Used to power the AI agents, including OpenAI and Ollama's models.

- Custom Internet Search Tool: Fetches information about flights, accommodations, and activities.
  
- Streamlit: Front-end framework for creating interactive web apps.
