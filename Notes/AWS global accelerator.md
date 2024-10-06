
- Improves global app availability and performance using AWS global network (60% improvement)
- Here request goes to an closest edge location from there request is routed through aws private network to direct host server.
- This way you can avoid many hoops and bounces in the public network.
- 2 anycast ip are created for the application and request is sent through edge location.

![[Pasted image 20240928200552.png]]