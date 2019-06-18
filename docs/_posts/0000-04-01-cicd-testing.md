# Test Automation
* Pipeline runs all tests
* ALL tests must pass

---
# Why?
* Users want working software
* We want automated deployment
* So we must automate testing

---
#Kinds of Test
* Developer Tests - CI
  * Is it built right?
  
* Deployment Tests - CD
  * Is it running right?
  
---
#Developer Tests
* Unit Tests
  * Is the logic right?
  
* Integration Tests
  * Is the system connected right?
  
* UI Tests
  * Is the look and feel right?
  
* Functional Tests
  * Is it working right?
  
---
#Deployment Tests
* Smoke Test
  * Is it deployed right?
  
* Health Checks
  * Is it running right?
  
* Sanity Checks
  * Does the happy path actually work live?
  
* Interesting: Netflix 'Chaos Monkey'
  * Do our failover systems actually work?
  
---
#Smoke Test
* Very simple for web apps
* Get an HTTP 200 OK from home page
* Use normal HTTP test tools
  * SpringBootTest
  * Rest Assured
  * Jest/Express

---
#EXERCISE: Build a Smoke Test
Write a smoke test for the Inspiration App

- Send an HTTP GET to /inspire
- Assert on receiving an HTTP 200 OK response  