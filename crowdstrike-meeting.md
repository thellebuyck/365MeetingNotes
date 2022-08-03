# CrowdStrike Demo Meeting

- Traditional AV vs EDR
  - WebRoot will take a bad file and give it a hashfile/Crowdstrike mostly looks for what the file is doing in the environment
- EDR use cases
- Crowdstrike Modules/Feature set with Falcon Complete
- Product Deployment and Management
- Hunting and incident analysis and response with Crowdstrike

- Conflict with WebRoot
  - Traditional AV (WR) has definitions update version
  - Crowdstrike doesn't have definition update version
  - Signs365 Systems have a sensor update policy (determines the version)
  - Exclusions in Crowdstrike for WebRoot.

- Crowdstrike Behavior-Based Detections
    - Builds confidence scores based on activities
    - Using and activity for determining malicious behavior.

## Management/Deployment

- CrowdStrike build group names:
- We currently have two groups: Servers/Workstations
- Policiies
  - Cautious - Will be certain that the process being killed won't affect the environment
  - Measured -
  - Active - if they are bad 
  
