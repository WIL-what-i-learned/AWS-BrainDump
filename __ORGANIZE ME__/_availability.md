# Availability

> running your application / system in at least 2 data centers (_availability zones_)

- 👀 usually goes hand in hand with horizontal scaling

## Auto Scaling

> launch TEMPLATES are recommended by AWS over launch CONFIGURATION 

- Livecycle hooks
    - enable you to perform custom actions by PAUSING instances as an Auto Scaling Group launches || terminates them
        - when instance is paused it remains in a `wait`

- Helper Scripts
    - used to install software and start services on an AWS ECT instance
        - `cfn-init` : retrieve and interpret metadata, insalled packages, create files, start services
        - `cfn-signal` : use `signal` with a CreationPolicy | WaitCondition do you can synchronize other resources in the stack while the prerequisite resource or application is ready
        - `cfn-get-metadata` : retrieve metadata for a resource || path to a specific key
        - `cfn-hup` : use check for updates to metadata and execute custom hooks when changes are detected

- Termination Policy
    - 

- Stress Test

- Scaling Policies
    - Auto Scaling Group has a metric and a Scaling Policy that is based on threshold of 

-

## Fauly Tolerance

## Data Recovery