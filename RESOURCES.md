# Amazon EKS Resources

## Knowledge

- [AWS Docs: Amazon EKS User Guide](https://docs.aws.amazon.com/eks/latest/userguide/)
  The canonical reference. Covers everything from cluster creation to node management. Start here for any EKS question.

- [AWS Docs: EKS Architecture](https://docs.aws.amazon.com/eks/latest/userguide/eks-architecture.html)
  Official overview of control plane and data plane architecture. Use for: understanding what AWS manages vs what you manage.

- [AWS Docs: Getting Started with EKS — eksctl](https://docs.aws.amazon.com/eks/latest/userguide/getting-started-eksctl.html)
  Step-by-step guide to creating a cluster with eksctl. Use for: first cluster creation.

- [AWS Docs: Getting Started with EKS — Console and CLI](https://docs.aws.amazon.com/eks/latest/userguide/getting-started-console.html)
  Manual cluster creation via console/CLI. Use for: understanding what eksctl automates.

- [AWS Docs: Create an Amazon EKS cluster](https://docs.aws.amazon.com/eks/latest/userguide/create-cluster.html)
  Detailed cluster creation reference (eksctl, console, AWS CLI). Use for: all cluster creation options.

- [AWS Docs: Self-managed nodes](https://docs.aws.amazon.com/eks/latest/userguide/worker.html)
  Overview of self-managed node groups. Use for: understanding custom AMI node deployment.

- [AWS Docs: Create self-managed Amazon Linux nodes](https://docs.aws.amazon.com/eks/latest/userguide/launch-workers.html)
  Launching self-managed node groups via eksctl or console (CloudFormation). Use for: deploying custom AMI nodes.

- [AWS Docs: Custom AMI support — eksctl](https://docs.aws.amazon.com/eks/latest/eksctl/custom-ami-support.html)
  How to use `--node-ami` and `amiFamily` with eksctl. Use for: deploying clusters with custom AMIs.

- [AWS Docs: Customize managed nodes with launch templates](https://docs.aws.amazon.com/eks/latest/userguide/launch-templates.html)
  Using launch templates for custom AMIs, user data, bootstrap args. Use for: node customization with managed node groups.

- [AWS Docs: AL2023 node bootstrapping with nodeadm](https://docs.aws.amazon.com/eks/latest/userguide/al2023.html)
  The new nodeadm YAML-based bootstrap process replacing bootstrap.sh. Use for: understanding how custom AMIs join EKS clusters.

- [AWS Docs: Build a custom EKS-optimized AMI](https://docs.aws.amazon.com/eks/latest/userguide/eks-ami-build-scripts.html)
  Open-source Packer scripts for building EKS AMIs. Use for: understanding what goes into an EKS node AMI.

- [GitHub: amazon-eks-ami](https://github.com/awslabs/amazon-eks-ami)
  Source of truth for EKS-optimized AMI builds. Contains bootstrap.sh, nodeadm, and Packer templates. Use for: understanding the exact node bootstrap process.

- [AWS Docs: EKS Best Practices Guide](https://docs.aws.amazon.com/eks/latest/best-practices/)
  Production-grade recommendations. Use for: security, networking, and operational best practices.

- [eksctl.io](https://eksctl.io/)
  Official eksctl documentation. Use for: CLI reference, config file schema, all eksctl features.

- [GitHub: eksctl-io/eksctl](https://github.com/eksctl-io/eksctl)
  eksctl source and documentation. Use for: config file examples, understanding what eksctl creates via CloudFormation.

- [AWS Docs: eksctl User Guide](https://docs.aws.amazon.com/eks/latest/eksctl/)
  AWS-hosted eksctl guide including tutorials and custom AMI support. Use for: step-by-step eksctl workflows.

## Wisdom (Communities)

- [r/aws](https://reddit.com/r/aws)
  Active subreddit with frequent EKS discussions. Use for: troubleshooting, community patterns.

- [AWS re:Post — EKS](https://repost.aws/tags/TA4IvCeWI1SkQNE5bUYgHKEg/amazon-elastic-kubernetes-service)
  AWS's official Q&A forum. Use for: specific error troubleshooting, known issues.

- [Kubernetes Slack — #eks](https://kubernetes.slack.com/)
  The `#eks` channel on Kubernetes Slack. Use for: real-time help from AWS engineers and community.

## Gaps

- No resource yet for bootc-specific AMI integration with EKS (likely needs primary research).
