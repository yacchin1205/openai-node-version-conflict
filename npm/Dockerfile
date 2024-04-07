# openai-node on pnpm
FROM node:20-slim

COPY . /app
WORKDIR /app

RUN npm install openai

# Run the test app
COPY ./test.js /app/test.js

CMD ["node", "test.js"]
