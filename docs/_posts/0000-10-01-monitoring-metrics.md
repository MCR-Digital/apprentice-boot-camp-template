#Monitoring and Metrics
As our system runs, we continuously measure its performance

---
# Why?
* Is it still working?
* Is it likely to fail soon?

--- 
#What do we monitor?
What things tell us about system health?

* Application logs - errors, fatal exceptions
* Request traffic - page views, urls
* Integration point availability
* CPU, RAM, Disk usage
* Response times - slowdowns may indicate trouble

---
#How?
Two aspects:
* Instrument our code
  * Strucutured Log output - decide what and where
  * Add measurement code - timing, counters
  
* Use reporting tools
  * ELK - Elasticsearch-Logstash-Kibana for distrubuted logs
  * AWS CloudWatch
  * Graphite and Grafana - graphing tools of metrics
  * Hystrix Dashboard - Integration points availability
  
---
#Alerting
Proactively tell us when something is out of line

* Examples
  * Response time > 10 seconds
  * Disk space > 90% used
* Send an email / SMS / Slack message

---
#Exercise: Add Monitoring and Alerting
Add basic uptime monitoring using www.uptimerobot.com

- Create a free account
- point it at the live URL of our app
- login to the dashboard and view
