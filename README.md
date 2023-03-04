RESOURCES 
- https://blog.devgenius.io/learn-rxjs-in-an-easy-way-8008f291ef8f
- share replay is used to prevent duplicate http requests. For example we have two obserbvables of courses which are advanced$ and beginner$, but each of them is tied to api calling all resources of courses. Since the both observables are lazily subscribed therefore when one of them is triggerd it will create a new http request instead of sharing the same one. With that share replay is needed
- behaviorSubject remembers the last value emitted by the subject or initial value. so any new subscribers will get the last value or initial value
