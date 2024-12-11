# AI-Powered Travel Planner using CrewAI Agents

This repository demonstrates how to use AI agents to create a comprehensive and personalized travel plan, including flight options, accommodations, activities, and itineraries. By leveraging LangChain, CrewAI and Streamlit for front end, you can simplify travel planning in a dynamic and interactive way.

To learn more about CrewAI Agents, please visit [CrewAI](https://docs.crewai.com/introduction).

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
