
- No servers to manage
- Limited by time  (short-execution)
- Run on-demand
- Scaling is automated
- It is event driven.


Features 
- Easy Pricing :
  - pay per request 
  - Free tier of 1M AWS lambda request and 400k GB-second of compute time.
- Integrated with many AWS services
- Easy monitoring using CloudWatch
- Support many languages 
  - Node
  - java
  - python
  - c#
  - Ruby
  - Custom Runtime API (community supported eg Rust or Golang)
  - Support Container Images (preferred ECS/Fargate)
- Easy to get more resources
- Increase ram will also increase CPU and Network.


Pricing
- Pay per call
  - First 1M call are free
  - $.02 per 1 M  request afterward
- Pay per duration: (in increment of 1 ms)
  - 400K GB-servond of compute time per month free
  - means if function uses 1GB ram then 400k seconds
  - if 2GM RAm then 200k seconds
  - AFter than $1 for 600k GB-second