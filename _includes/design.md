- Communication between Jenkins and Gerrit happens through ssh. The difficulty of
  managing ssh keys is removed by deploying through this template.
- The gerrit-trigger plugin is automatically configured to allow Gerrit to
  stream code review events to Jenkins to trigger jobs.
- SSL termination is offloaded to apache on both the Gerrit and Jenkins
  nodes.
- Gerrit authentication is configured to use Ubuntu SSO making Gerrit user
  account management simple.
- Network isolation and security group isolation at various levels within
  the stack provide enhanced Cloud security.
