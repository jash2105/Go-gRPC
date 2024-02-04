# grpc-go-chatgpt: Empowering Server-Client Communication with Go, ChatGPT, and gRPC

## Introduction

Welcome to `grpc-go-chatgpt`, an advanced project that revolutionizes server-client communication by harnessing the capabilities of Go, ChatGPT, and gRPC. This cutting-edge solution is designed for rapid and dependable interactions between servers and clients, leveraging the formidable `gpt-3.5-turbo` model through the OpenAI API, all within the Go programming ecosystem.

## The Driving Force

`grpc-go-chatgpt` emerged from the essential need to seamlessly integrate OpenAI's API with custom server-side features and transmit data efficiently to the frontend. This project emphasizes prompt engineering and rule-based systems, making it a powerful tool for developers tackling similar challenges in their own projects and scenarios.

## Containerization and Deployment



Before you proceed, please ensure that Docker is installed on your machine. 

1. Ensure Docker is installed on your machine. If not, download it from [here](https://docs.docker.com/get-docker/).

2. Clone this repository to your local environment.

3. Add your OpenAI API key to the `docker-compose.yml` file:

   ```bash
   environment:
     - OPENAI_KEY=your-openai-key-is-here
   ```

4. In the project's root directory, execute the following command to set up the Docker environment and build the necessary components:

   ```bash
   docker-compose build
   ```

   This process may take a few minutes to complete.

5. Once the build is finished, run the following command to launch `grpc-go-chatgpt`:

   ```bash
   docker-compose up -d && docker attach go-grpc-client
   ```

