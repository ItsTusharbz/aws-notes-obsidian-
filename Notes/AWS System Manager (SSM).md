
- It is a ==hybrid service== to manage the EC2 or on-premise system
- Important features
  - Patching automation for compliance
  - Run commands across all the system at once
  - Store parameter configuration with SSM parameter store
- Works for Linux, windows, MacOs and Raspberry Pi os 

How it works
- Install SSM agent onto the systems we control
- These agent will send event to AWS

#### SSM Session Manager

- Allow you to start session with the connected (SSM agent installed) resources ( eg EC2 or on-premise server).
- No SSH, Bastion hosts or SSH keys required.
- No port 22 needed.
- Support Linux, macOs and windows
- Send session logs to s3 or cloudWatch


#### SSM Parameter keys
- Using this we can create parameter in SSM to be used in the session
- to use saved parameter in session use command `{{ssm:parameter-name}}` and get the value
- Parameter Store provides support for three types of parameters: `String`, `StringList`, and `SecureString`.