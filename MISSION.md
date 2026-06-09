# Mission: Amazon EKS

## Why
I'm developing a bootc container image that will be converted into a custom AMI for use as Kubernetes nodes in an EKS cluster. I need to understand EKS well enough — both console and CLI — to create clusters, configure node groups with custom AMIs, and validate that my bootc-based nodes work correctly in that environment.

## Success looks like
- Create an EKS cluster from scratch (console and CLI)
- Configure a node group that uses a custom AMI
- Validate that a custom-AMI node joins the cluster and runs workloads
- Understand EKS networking, IAM roles, and node lifecycle well enough to debug issues when a custom node doesn't behave as expected

## Constraints
- Using a work AWS account (be mindful of costs — tear down resources after exercises)
- Comfortable with Kubernetes already — don't need pod/service/deployment basics
- Light AWS experience — need to learn relevant AWS primitives (IAM, VPC) as they come up
- Want to learn both the web console and CLI workflows

## Out of scope
- Kubernetes fundamentals (already known)
- EKS add-ons deep dives (Fargate, App Mesh, etc.) unless directly relevant to node management
- Building the bootc image itself (that's a separate effort)
