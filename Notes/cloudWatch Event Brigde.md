- Every service in AWS triggers an event which gets send to cloud watch event. Using those events we can schedule or trigger a target, or set an action (eg trigger SNS topic to send email).
- There are 2 types of rules
  1. Pattern based
  2. cron job (time based)
- model event schema
- archive events (all/filter) 
- ability to play events.
### Event bus
- using event bus you can send event from third party application or your own app to AWS event bridge.

![[Pasted image 20241011184712.png]]