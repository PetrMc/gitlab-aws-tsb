# The simple pipeline example to support CI/CD gitlab pipeline blue/green deployment to AWS using Tetrate Service Bridge (TSB)

Pre-req's
- all variables and DynomoDB setup from the pipeline explained here https://aws.amazon.com/blogs/containers/ci-cd-with-amazon-eks-using-aws-app-mesh-and-gitlab-ci/
- Application namespace `tetrate-demo' is created
- FQDN for application exists
- TSB Management (in any environemt on prem, other clouds)  and control plane(s) deployed in AWS EKS
- TSB Workspace, Gateway Group, Traffic group objects are created
- TSB Password (TSB_PASS), TSB URL (TSB_FQDN) and Tenant (TSB_TENANT) are defined in the pipelie
- ECR repo called `tetrate-app` is created
- IAM user created in the above steps has kubernetes access to application cluster - per https://docs.aws.amazon.com/eks/latest/userguide/add-user-role.html

The demo video of the final result can be seen here: https://youtu.be/1dsijHzp2UA (unedited version here - https://www.youtube.com/watch?v=OQGtnlCELoY )
