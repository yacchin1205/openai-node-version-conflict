# openai-node on pnpm
FROM node:20-slim

# Install pnpm
ENV PNPM_HOME="/pnpm"
ENV PATH="$PNPM_HOME:$PATH"
RUN corepack enable
COPY . /app
WORKDIR /app

RUN pnpm install openai

# Run the test app
COPY ./test.js /app/test.js

CMD ["node", "test.js"]
