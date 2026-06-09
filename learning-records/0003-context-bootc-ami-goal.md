# Context: Building a bootc-based custom AMI for EKS nodes

User is developing a bootc container image (see https://containers.github.io/bootable/) that will be converted into a custom AMI for use as EKS worker nodes. This means lessons should eventually cover: self-managed node groups, custom AMI bootstrap requirements (nodeadm for AL2023-era), launch templates, and the specific requirements an AMI must satisfy to join an EKS cluster. The bootc image build itself is out of scope.
