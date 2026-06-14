# Bootc image will ship nodeadm and containerd

User decided to ship nodeadm and containerd in the bootc AMI rather than using CRI-O with a custom bootstrap. This simplifies the EKS integration significantly: the bootc AMI can use `amiFamily: AmazonLinux2023` in eksctl, and eksctl will auto-generate the correct NodeConfig user data. nodeadm on the bootc image will parse it and bootstrap the node identically to an official AL2023 AMI. This supersedes the earlier assumption in learning record 0006 about CRI-O being the target runtime.
