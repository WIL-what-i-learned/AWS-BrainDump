# AWS - Elastic Container Service (ECS)

## Comparison to Elastic Kubernetes Service

| EKS Concent                   | ECS Comparison                | 
| ---                           | ---                           |
| Rod                           | Task                          | 
| Replicaset + Service          | Service                       |
| Horizontal Pod Autoscaler     | Task auto scaler              |   
| Cluster autoscaler            | Capacity provider scaling     |  


## Launch Types

- [EC2](../../../_compute/EC2_ElasticComputeCloud/README.md)
- Fargate

## Notes

- LOGGING: integrated with `CloudWatch` out of the box
- MONITORING: integrated with `CloudWatch` out of the box

