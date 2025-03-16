# QuickBooks Voice Invoice App

A web application that allows users to create QuickBooks invoices using voice commands.

## Features

- Voice-to-text conversion for creating invoices
- Integration with QuickBooks Online API
- User authentication and authorization
- Secure storage of user data and QuickBooks tokens
- Responsive web interface

## Tech Stack

- **Frontend**: React, TypeScript, Tailwind CSS
- **Backend**: Node.js, Express
- **Database**: MongoDB
- **Authentication**: JWT
- **Voice Processing**: OpenAI Whisper API
- **Natural Language Processing**: OpenAI GPT API
- **Containerization**: Docker

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- Docker and Docker Compose
- MongoDB (if running without Docker)
- QuickBooks Developer Account
- OpenAI API Key

### Environment Setup

1. Clone the repository
2. Copy `.env.template` to `.env` and fill in your credentials
3. Set up your QuickBooks Developer account and create an app to get API credentials

### Running with Docker

```bash
docker-compose up -d
```

This will start the MongoDB database, backend API, and frontend application.

### Running without Docker

#### Backend

```bash
cd backend
npm install
npm run dev
```

#### Frontend

```bash
cd frontend
npm install
npm run dev
```

## API Documentation

API documentation is available at `/api-docs` when the server is running.

## Security Considerations

- All API keys and secrets should be stored in the `.env` file (not committed to version control)
- QuickBooks tokens are encrypted before being stored in the database
- Rate limiting is implemented to prevent abuse
- CORS is configured to only allow requests from the frontend

## License

MIT