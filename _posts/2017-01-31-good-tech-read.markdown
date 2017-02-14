---
layout: post
title:  "Good Tech Read"
date:   2017-01-31 21:11:41 -0800
categories: tech read
---
### [JVM GC flags][jvm-gc]
- GC's goal: min pauses & max throughput
- Pause happens when
  - thread switch context
  - GC thread searches for unreferenced object in heap
- Frequent GC: small pauses, small throughput
- Unfrequent GC: big pauses, big throughput
- `-XX:+UseSerialGC`
  - single-threaded GC for single thread service
- `-XX:+UseParallelGC`
  - multi-threaded GC for java >=7
- `-XX:+UseParallelOldGC`
  - includes young and old generation of GC
  - for multi-core processors
  - preferred over +UseParallelGC
- `-XX:ParallelGCThreads=<N>`
  - specify threads for parallel GC
  - `N=Runtime.availableProcessors()`
  - if `N<8`, use `N`; else use `3+5N/8`

### [JavaScript Callback Mechanism][callback]
![callback]({{ site.url }}/assets/callback.png)

### [Li Feifei Ted Talk][ml]
![ml]({{ site.url}}/assets/convolutional-neural-network.png)

[jvm-gc]: https://blog.codecentric.de/en/2013/01/useful-jvm-flags-part-6-throughput-collector/
[callback]: https://www.youtube.com/watch?v=8aGhZQkoFbQ
[ml]: https://www.youtube.com/watch?v=40riCqvRoMs
