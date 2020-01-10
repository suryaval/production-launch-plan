# Launch Planning Phases

## Start Launch Planning Early

* Some early feedback might help in re-architecture of the product that aligns with user's expectations

## Get Traffic Projections

* Demand for the product (How many operations per unit of time/ requests per second or per hour)

* Traffic estimates: no. of users/peak times for traffic spikes
    *   traffic during day-of-launch
    *   traffic during near-term-range : 1-week
    *   traffic during middle-term-range : 1-month
    *   traffic during long-term-range : 6-12 months

* What is the database usage? transactions/writes

## Review Product Architecture

* Get the diagrams of how the product’s components interact and what they depend on

* Every software entity has some API and an owner who ensures that API delivers its function

* This point in launch planning is where you extract who the points of contact are

* what service-level objectives (SLOs) are provided

* what RPCs your product sends, and how much resources of various types those RPCs cost

* Is there any data corruption risk

## Risks & Mitigations Table

|Risk Area|Risk Description|Failure Mode|Mitigation Strategy|Status|
|:-------:|:--------------:|:----------:|:-----------------:|:----:|
|Cloud Service Provider ex: AWS AZ down|API requires AWS SNS|User cannot use API|Graceful Handling is required|High Risk - Pending|

## Evaluate the User Experience

* Enable telemetry from the services
    *   How many 400x does the API issue?
    *   What is the API Latency?
    *   

