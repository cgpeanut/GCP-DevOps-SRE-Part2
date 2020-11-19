# GCP-DevOps-SRE-Part2
https://learn.acloud.guru/course/1c5c969b-7881-47e9-a7d1-b4a7c65cbe67/dashboard

chapter 2: Balancing change, velocity, and service reliability with SREs
- Big Picture: What is Site Reliability Engineering? 
  -  Team DEV - new features getting to market quicky
  -  Team OPS - goal s smoothly BUT new features breaks the smooth operation
DevOps - A software engineering culture and practice, that aims at unifying software development and software operations.

DevOps infinity Loop:
[<img src="https://github.com/cgpeanut/GCP-DevOps-SRE-Part2/blob/main/data/infinity_loop.png">]

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

class SRE Implements DevOps
