# Lab 8 - Containerize Spring Boot App (build inside Docker)

## Objective
Build the Spring Boot app inside a Maven-based Docker image and run it from a lightweight JDK image.

## Commands
- Build image (from project root):
  ```bash
  docker build -t lab8-app -f Dockerfile .
  ```
- Run container:
  ```bash
  docker run -d -p 8080:8080 lab8-app
  ```
- Test:
  ```bash
  curl http://localhost:8080/
  ```
