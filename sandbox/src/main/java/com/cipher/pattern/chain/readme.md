## 责任链模式

### 概念
将接收者对象（Handler，持有一个自身类型的引用）连成一条链，并在该链上传递请求，直到有一个接收者对象处理它。
通过让更多对象有机会处理请求，避免了请求发送者(Client)和接收者之间的耦合。

发出请求的客户端并不知道链上的哪一个接收者会处理这个请求，从而实现了客户端和接收者之间的解耦。

开闭原则：对扩展开放，对变更关闭。

缺点：时间、内存

应用：Java异常机制、JS事件机制、Java Web过滤器Filter(Spring Security)