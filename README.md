# Ketchapp - Real-time Chat Application  

## Overview

Ketchapp is a fully real-time user interaction platform that increases active user engagement by approximately 30% and supports over 100 simultaneous users. This is achieved by leveraging a serverless, event-driven architecture using React (with useEffect hooks) and WebSocket on the AWS CloudFront network. Additionally, the application integrates intelligent agentic moderators via Groq API to automate conversation management and streamline user interactions.

### Live Demo

[Click here to access the live demo](https://staging.d1389o6r6x8bes.amplifyapp.com/)

## Features

- Real-time communication with WebSockets
- User presence tracking
- Public and private messaging
- Serverless architecture for scalability
- AI-powered chatbot moderation using Groq API
- Persistent chat logging to AWS S3

## Technologies Used

- **Frontend:** React (useEffect, useState, useRef)
- **Backend:** AWS Lambda, API Gateway, WebSocket
- **Cloud Services:** AWS CloudFront, S3
- **AI Integration:** Groq API

## Setup and Installation

### Prerequisites

- Node.js (>= 14.x)
- AWS CLI configured with necessary permissions
- Groq API key

### Backend Setup

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/ketchapp.git
   cd ketchapp
   ```
2. Deploy the AWS Lambda function and API Gateway WebSocket:
   - Update `ENDPOINT` in `lambda_handler.py` with your API Gateway WebSocket URL.
   - Ensure `S3_BUCKET_NAME` is set to your AWS S3 bucket name.
   - Deploy using AWS CLI or Terraform (if applicable).

### Frontend Setup

1. Navigate to the frontend directory:
   ```sh
   cd frontend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Set environment variables:
   ```sh
   echo "REACT_APP_API_KEY=your_groq_api_key" > .env
   ```
4. Start the development server:
   ```sh
   npm start
   ```

## Usage

1. Open the application and enter a username.
2. Click **Connect** to join the chat.
3. Send public messages or private messages to specific users.
4. Mention the bot (`@RoBot`) in your message to get AI-generated responses.

## Deployment

To deploy the frontend using AWS Amplify:

```sh
amplify init
amplify add hosting
amplify publish
```

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch (`feature-branch`).
3. Commit your changes.
4. Push to the branch and submit a pull request.

## License

This project is licensed under the MIT License.

## Contact

For any queries, contact [your email or GitHub profile link].



