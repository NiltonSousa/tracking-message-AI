# Tracking Message AI

This project show how to do a simple route to integrate openAI to ask questions and receive response.

## How to use

Create .env file using .env.example and fill OPENAI_API_KEY with your api key.

.env file

```bash
OPENAI_API_KEY=your-api-key
```

Install dependencies

```bash
npm ci
```

Start server

```bash
npm run dev
```

## Routes

POST /message

```bash
curl --location 'http://localhost:3000/message' \
--header 'Content-Type: application/json' \
--data '{
    "message":"Olá, meu nome é nilton"
}'
```

Example response

```bash
{
    "content": "Olá, Nilton! Como posso ajudá-lo hoje?"
}
```
