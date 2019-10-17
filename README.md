# **Campr Vulnerable Components Workshop**

## **Running in Local Machine**

---

## Requirements

- JDK 1.7 or 1.8
- A Java IDE

## Steps

- [Optional] Generate Intellij project files:

  ```bash
  ./gradlew idea
  ```

- Run the application

  ```bash
  ./gradlew appRun
  ```

## **Running in Docker**

---

## Requirements

- Docker desktop > 2.1
  ```bash
  brew cask install docker
  ```
- A Java IDE

## Steps to complete the workshop

1. Run the application

   ```bash
   docker-compose rm -f && docker-compose up
   ```

2. Open the application & find the bug http://localhost:8080/

3. Fix the bug in the code

4. Restart the application
   ```bash
   docker-compose rm -f && docker-compose up
   ```
5. Open the application & verify the bug is fixed http://localhost:8080/

6. Stop the application
   ```bash
   docker-compose down
   ```
