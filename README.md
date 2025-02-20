# IOT-BASED-WEATHER-MONITORING-
# IoT-Based Weather Monitoring Dashboard

This project demonstrates an IoT-based weather monitoring system that uses IBM Cloud Functions to process real-time weather data from IoT devices and displays it dynamically on a React.js front end.

## Overview

The system collects weather parameters (such as temperature, humidity, and pressure) from various IoT devices and processes the data using IBM Cloud Functions in a serverless environment. The processed data is then sent to a back-end server built with Node.js (using Express and Socket.IO), which provides both a REST API for historical data and real-time updates. Finally, a React.js dashboard visualizes this data interactively using Axios for API calls and Recharts for charting.

## Features

- **Real-Time Data Processing:** Uses IBM Cloud Functions to process and handle incoming IoT weather data.
- **Dynamic Dashboard:** A React.js application that displays weather data in real time using charts and live updates.
- **REST API:** Provides endpoints to retrieve historical weather data.
- **Real-Time Updates:** Implements Socket.IO for broadcasting live weather updates to connected clients.
- **Cloud Integration:** Integrated with IBM Watson IoT Platform for device registration and data ingestion.

## Architecture

The project consists of three main components:

1. **IoT Devices:** Sensors (e.g., ESP32, Raspberry Pi) that collect weather data and send it to the cloud.
2. **Back-End Server:**
   - A Node.js server using Express to provide REST APIs.
   - Socket.IO for broadcasting real-time data updates.
   - CORS-enabled to allow cross-origin requests from the React app.
3. **Front-End Dashboard:**
   - Built with React.js.
   - Uses Axios to fetch historical weather data.
   - Visualizes data using Recharts.
   - Listens for real-time updates via Socket.IO.

## Project Structure

