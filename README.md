# NewRelic

New Relic	

Observability 
- Collection of metrics data  -  Telemetry
- Why important - move from Monolithic to micro services

Questions to ask:
- Is the service on ?
- Is the service functioning as expected?
- Is the service performing well ?

MTTD - Mean Time to Detection
MTTR -  Mean Time to Recovery

UI Layer -  Core Web Vitals 
	-  LCP - Largest Contentful Paint(Pageload), 
	- FID - First Input delay(responsiveness), 
	- CLS - Cumulative Layout Shift(Stability)
Service Layer  - RED Method (Rate - Request/sec, Errors, Duration - Latency) -  Request Oriented
Infrastructure Layer - USE Method (Utilization, Saturation(Network Queue), Errors

Four Golden Signals Method(RED+S) -  Latency, Traffic, Errors, Saturation - by Google

Types of Telemetry - MELT(Metric, Event, Logs, Traces)

Instrumenting to gather metrics via agents
- APM Agents(Application Performance Monitoring)
- Browser Agents
- Mobile Agents
- Infrastructure Agents

NRDB - New Relic Data Base - No SQL Database with out any schema, Contains router and worker nodes for processing queries 

- Everything in New Relic is an entity with unique ID and these can be tagged/grouped.
- For Python, we can install new relic with PIP3 Install newrelic - will install newrelic agent and consumes the newrelic.ini config file which has license key, app_name …etc(NEW_RELIC_CONFIG_FILE need to be set with config file name 

New Relic Console
- All Entities - categorized as services host and other details
    - Different Views
        - List - select an entity -> service Map (to get outline of UI/Services/Infra layout for that service)
        - Navigator - hexagon view with Red- issue, Green - all good, gray - not reporting to newreelic
        - Lookout  - which has Metrics info RED/USE…
- Browser -  for any UI components - tracks core web vitals, Error rates
- ApDex -  measures users satisfaction level. - Application Performance Index(between 0(worst) and 1(best)) = (Satisfied Requests + (Tolerating Requests/2))/Total number of requests 
    - Response time < = Threshold -  satisfied
    - Response time > Threshold -  Tolerating
    - Response time > 4 X Threshold -  Frustrated
      
