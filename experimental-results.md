Experimental Results

Researcher: Kimora McLemore
Date: November 18, 2026
Environment: GitHub Actions and Kubernetes in Docker (Kind)
Kubernetes Version: v1.32.0

Deployment Results

The Kubernetes cluster was successfully created in 41 seconds. The infrastructure deployment was completed in 4 seconds. One application replica was running with zero restarts at the time of inspection. The complete GitHub Actions workflow took 55 seconds.

Security Control Results

Role-based access control (RBAC) was implemented using two separate service accounts. The authorized service account passed the permission check, while the unauthorized service account was denied permission to retrieve the research secret.

The application also successfully received the synthetic test credential through a Kubernetes environment variable.

Limitations

The experiment was conducted using a temporary Kubernetes cluster rather than Amazon EKS due to AWS access limitations. One experimental run was completed. AWS Secrets Manager and Sealed Secrets were not experimentally evaluated in this run.

The results demonstrate the functionality of native Kubernetes Secrets and RBAC under the tested conditions but do not establish comparative performance across all three methods.

AI Disclosure

ChatGPT assisted with infrastructure code, experimental workflow development, and documentation. The reported results were obtained from the executed GitHub Actions workflow.
