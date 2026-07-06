Ques: What is PVC in AWS?

Ans:- PVC is a Kubernetes resource that requests persistent storage. In AWS, it is typically backed by Amazon EBS for block storage or Amazon EFS for shared storage, ensuring application data persists even if pods are recreated.

Ques: Which Services are used in AWS?

Ans:- In AWS, PVC is typically backed by Amazon EBS for block storage and Amazon EFS for shared file storage. Kubernetes uses the AWS CSI drivers to dynamically provision these storage volumes.

Ques: Why do we use IAM?

Ans:- IAM is used to securely control access to AWS resources by managing users, groups, roles, and permissions, ensuring only authorized users or services can perform specific actions.

Ques: What are the Groups and Roles in IAM?

Ans:- An IAM Group is used to assign common permissions to multiple users, while an IAM Role provides temporary permissions that users or AWS services can assume to access AWS resources securely.

Ques: Difference b/w IAM Group & IAM Role?

Ans:-
| S.No | IAM Group                                               | IAM Role                                                                       |
| ---- | ------------------------------------------------------- | ------------------------------------------------------------------------------ |
| 1    | Assigned to IAM users                                   | Assumed by IAM users or AWS services                                           |
| 2    | Used to manage permissions for multiple users           | Used to grant temporary permissions                                            |
| 3    | No temporary credentials                                | Uses temporary security credentials (STS)                                      |
| 4    | Cannot be attached directly to EC2, Lambda, EKS, or ECS | Can be attached to EC2, Lambda, EKS, ECS, and other AWS services               |
| 5    | Users become permanent members of a group               | Roles are assumed only when needed                                             |
| 6    | Best for managing permissions of multiple IAM users     | Best for service-to-service access, cross-account access, and temporary access |

