- Automated Security Assessments
- For EC2
  - Leverage System Manager agent (SSM)
  - Network reachability.
  - unintended network access
  - Running Os and known vulnerabilities
-  Lambda
  - software vulnerability in function code and package dependancy 
- Docker container pushed to ECR
- Reporting & integration with AWS security hub
- Send finding to Amazon Event Bridge.
- Inspector checks the database of CVE(publicly reported vulnerability database) (https://www.cve.org/) and check if those vulnerability exists in EC2, Lambda code or ECR packages 
- Gives risk score to vulnerability bases on severity.

