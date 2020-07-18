# **Campr Vulnerable Components Workshop**

## **Running in Docker**

---

## Requirements

- Docker desktop > 2.1
  ```bash
  brew cask install docker
  ```
- A Java IDE _e.g, IntelliJ IDEA_ (an IDE is recommended, not mandatory. An editor will do just fine, if you are comfortable with it)

## Steps to complete the workshop

1. Run the application

```
  git clone https://github.com/AppSec101/campr-vulnerable-components.git
```

(ignore the above step if already cloned)

```
  cd campr-vulnerable-components
```

```bash
docker-compose rm -f && docker-compose up
```

2. Open the application at http://localhost:8080/

3. Identify the vulnerable depdendency and upgrade it

4. Once the test passes, Restart the application
   ```bash
   docker-compose rm -f && docker-compose up
   ```
5. Open the application & verify the bug is fixed http://localhost:8080/

6. That's it. Stop the services and do clean up.
   REMEMBER TO DO THIS STEP. LEAVING THE SERVER RUNNING COULD PUT YOUR COMPUTER AT RISK DUE TO THE VULNERABLE APPLICATION

   ```bash
   docker-compose down
   docker-compose rm -f
   ```

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

- Open the app at http://localhost:8080/

- Run the tests. All tests will pass

  ```bash
  ./gradlew test
  ```
