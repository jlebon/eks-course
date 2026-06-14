# CRI-O is a viable runtime for EKS nodes, but bypasses nodeadm

kubelet supports any CRI-compliant runtime (containerd, CRI-O). However, EKS's `nodeadm` tool is hardcoded to manage containerd. Using CRI-O means either skipping nodeadm entirely and writing a custom bootstrap mechanism, or working around nodeadm's containerd assumptions. For a bootc/RHEL-based AMI that ships CRI-O, the custom bootstrap path is likely the right approach with self-managed node groups.
