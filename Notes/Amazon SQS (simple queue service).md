
![[Pasted image 20240930171253.png]]


- This is a simple queue service which takes message in (producer) and consumer will subscribe to it. 
- It is used to decouple producer and consumers.
- Once the message is consumed it will be deleted.
- Maximum storage duration is 4 days to 14 days
- No maximum storage capacity
- can scale from 10msg /sec to 10000 msg/sec.
- Consumer share the work to read messaged and scale horizontally.


FIFO Queue
- Here message order is maintained First In First Out.