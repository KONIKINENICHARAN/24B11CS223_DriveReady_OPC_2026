# Task: Indian Railway Passenger Assistant Chatbot

## Task Description

Develop an AI-powered chatbot using the Groq API to assist passengers with information and awareness related exclusively to Indian Railways passenger services.

The chatbot is designed to answer passengers' queries about train ticket booking, PNR status, RAC, Waiting List, Tatkal booking, ticket cancellation, refund procedures, railway rules, baggage regulations and passenger facilities while restricting unrelated conversations.

## Implementation

- Installed the required Python libraries, including `groq` and `python-dotenv`.
- Loaded API credentials securely from the `.env` file, with a secure manual API key input option.
- Initialized the Groq client to interact with the `openai/gpt-oss-20b` model.
- Designed a detailed **System Prompt** defining the chatbot's role, responsibilities, allowed topics and restricted topics.
- Implemented topic validation instructions to ensure that the chatbot responds only to Indian Railway passenger-related queries.
- Configured the chatbot to provide information about ticket booking, PNR status, RAC, Waiting List, Tatkal booking, cancellations and refunds.
- Implemented conversation memory using a messages list containing system, user and assistant messages.
- Maintained conversation history by passing previous messages along with every new request to the AI model.
- Configured model parameters such as temperature and maximum response tokens.
- Implemented support for simple English and Telugu.
- Implemented a continuous chatbot loop to accept multiple passenger queries.
- Added exit commands (`quit`, `exit`, `bye`) to terminate the conversation.
- Implemented exception handling to manage API errors and remove failed user messages from conversation history.
- Designed a predefined response for questions unrelated to Indian Railways.

## Key Concepts Implemented

- Groq API Integration
- System Prompt Engineering
- Role-Based AI Behavior
- Topic Restriction and Validation
- Conversational Memory
- Chat Completion API
- Exception Handling
- Interactive CLI-Based Chatbot
- Environment Variable Management
- Multilingual AI Responses
