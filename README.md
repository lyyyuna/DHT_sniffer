DHT 公网嗅探器
===========

这是根据 DHT 协议写的嗅探器，下载种子的 infohash。另外我还写了 [Go 版的 DHT 嗅探器](https://github.com/lyyyuna/godht)。

其实暂时大部分代码来自了 [simDHT](https://github.com/Fuck-You-GFW/simDHT/blob/master/simDHT.py)，我只是改成了 gevent 版本。因为原来的版本虽然是多线程，但是在 udp.recv 的时候还是会阻塞的。

## 简单说明

### 依赖

* Python 2.7
* pip install gevent
* pip install bencode