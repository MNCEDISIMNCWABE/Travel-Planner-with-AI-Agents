# AI-Powered Travel Planner using CrewAI Agents

This repository demonstrates how to use AI agents to create a comprehensive and personalized travel plan, including flight options, accommodations, activities, and itineraries. By leveraging LangChain, CrewAI and Streamlit for front end, you can simplify travel planning in a dynamic and interactive way. In this repo, I used CrewAI as the main framework because it allows the use of tools with almost any open-source LLM. 

To learn more about CrewAI Agents, please visit [CrewAI](https://docs.crewai.com/introduction).

## Setup

### Prerequisites

- LLM Server: This server is responsible for running inferences using the selected language model (LLM). It can operate as a remote server, such as OpenAI’s service, or as a locally hosted instance. Install [Ollama](https://ollama.com/) to run LLMs locally. Alternatively, you can use any local LLM server such as[ LM Studio](https://lmstudio.ai/), but this project specifically uses Ollama.

- Create an account with [Serper API ](https://serper.dev/) to obtain an API key for internet search functionality, you will get 2500 free searches.

## Features

1. Two AI Agents:

- Travel Planner: Finds relevant information about budget-friendly flights, accommodations, and activities to do at destination from the internet.

- Vacation Itinerary Creator: Crafts a detailed, day-by-day itinerary based on the Travel Planner's agent findings.

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

- Crew.AI: Simplifies multi-agent task execution.

- LLMs (Language Learning Models): Used to power the AI agents, including OpenAI and Ollama's models.

- Custom Internet Search Tool: Fetches live data for flights, accommodations, and activities.
  
- Streamlit: Front-end framework for creating interactive web apps.
