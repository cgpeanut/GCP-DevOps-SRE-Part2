# GCP-DevOps-SRE-Part2


https://learn.acloud.guru/course/1c5c969b-7881-47e9-a7d1-b4a7c65cbe67/dashboard

chapter 2.1: Balancing change, velocity, and service reliability with SREs
- Big Picture: What is Site Reliability Engineering? 
  -  Team DEV - new features getting to market quicky
  -  Team OPS - goal s smoothly BUT new features breaks the smooth operation
DevOps - A software engineering culture and practice, that aims at unifying software development and software operations.

DevOps infinity Loop:
[<img src="https://github.com/cgpeanut/GCP-DevOps-SRE-Part2/blob/main/infinity_loop.png">]

Key Pillars of DevOps
    
    Reduce Organizational Silos:
        - Bridge teams together
        - Increase communication
        - Share company vison - along the way accept failure as normal.
        - Incidents bound to occur. 
        - Failure help team learn
  
    Implement gradual change
       - Small updates are better 
       - Easier to review
       - Easier to rollback

    Leverage Tooling & automation
       - Reduce manual task
       - The heart of CI/CD pipelines
       - Fosters sopeed & consistency
    
    Measure Everything
       - Critical gauge of success
       - CI/CD needs full monitoring 
       - Synthetic, proactive monitoring

Site Reliability Engineering (SRE) - what happens when a software engineer is tasked with what used to be called opeations.

Why reliabilty ?
    - most important: does the product work ?
    - Reliability is the absence of errors.
    - Unstable service likely indicates a variety of issues. 
    - Must attend to reliability all the time - not justr when there is your hair is on fire. 

class SRE(The How) Implements DevOps (The What!)

Key Pillars of DevOps + SRE

    Share Ownership
      - Developers + Operations
      - Implement same tooling (Jenkins, ansible, terraform) - Jira/azure devops (Project mgmt)
    Accept failure as normal 
      - Try not to anticipate, but...
      - Incidents bound to occur
      - Failures help team learn
            No-fault post mortems & SLOs 
              - No Two failures the same 
              - Track incidents (SLIs)
              - Map to Objectives (SLOs)
    Implement gradual change
      - small updates are better
      - easier to review
      - easier to rollback
             Reduce cost of failures
              - limited "'canary" rollouts - test small portions of user the gradually expand the user base.
              - impact fewest users
              - automate where possible
    Leverage tooling and automation
      - Reduce manual tasks
      - The heart of CI/CD pipelines
      - Fosters speed and consistency
            Automate this year's job away
                - automation is a force multiplier
                - autonomous automation best
                - centralizes mistakes
    Measure everything
      - critical gauges of success
      - CI/CD needs full monitoring 
      - synthetic, proactive monitoring 
            Measure toil and reliability
                - key to SLOs and SLAs
                - reduce toil, up engineering

To sum up: SRE Overall goal is to make better software faster!
[<img src="https://github.com/cgpeanut/GCP-DevOps-SRE-Part2/blob/main/sre-goal.png">]

SRE: Site Reliability Engineering 
1.  define availability
2.  determine level of availability
3.  plan in case of failure

chapter 2.2: Understanding SLIs (service level indicators)

SRE: Site Reliability Engineering 
1.  define availability
    - SLO: service level objective
2.  determine level of availability <>
    - SLI: service level indicator
3.  detail what happens when availability fails
    - SLA: service level agreement 

SLI: " a crefully defined quantitative measure of some aspect ofg the level of service that is provided."
SLIs are metrics over time - specific to a user journey such as request/response, data processing, or storage - that show how well a service is doing. 
    example SLIs:
        - Request latency - how long it takes to return a response to a request.
        - failure rate - a fraction of all rates received: (unsuccessful requests/all requests).
        - batch throughput - proportion of time - data processing rate > than a threshold.

