# Email AI - Full Stack Email Reply Generator

This project is an AI-powered application that generates professional or casual email replies using Google Gemini.

## Project Structure
- **Root**: Frontend (React + Vite + Material UI)
- **`email-writer-sb/`**: Backend (Spring Boot + Spring AI + Vertex AI Gemini)

## Features
- Paste any email content and get a generated reply.
- Select from multiple tones (Professional, Casual, Friendly).
- One-click "Copy to Clipboard" functionality.

## Prerequisites
- Java 23
- Node.js & npm
- Google Cloud Project with Vertex AI API enabled

## Running the Application

### 1. Backend (Spring Boot)
1. Authenticate with Google Cloud:
   ```bash
   gcloud auth application-default login
   ```
2. Set your Project ID:
   ```bash
   # Windows PowerShell
   $env:GCP_PROJECT_ID="your-project-id"
   ```
3. Run the application:
   ```bash
   cd email-writer-sb
   ./mvnw spring-boot:run
   ```

### 2. Frontend (React)
1. Install dependencies:
   ```bash
   npm install
   ```
2. Run in development mode:
   ```bash
   npm run dev
   ```

## Technologies Used
- **Frontend**: React, Vite, Material UI (MUI), Axios
- **Backend**: Spring Boot 3.4, Java 23, Spring AI, Google Vertex AI (Gemini 1.5 Flash)
