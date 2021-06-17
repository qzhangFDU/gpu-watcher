# gpu-watcher

![mark](http://qizhang.info/gpu-watcher.png)

## 依赖

python3

client:
```bash
pip install pyyaml pynvml
```

server:
```bash
pip install pyyaml pynvml flask
```

## 使用方式

修改 `config.yaml`

```yaml
lab:
  center:
    ip: 202.204.62.145 // 中心节点的ip和端口（汇总GPU信息用）
    port: 80

local:
  host: G1_4GTX1080Ti // 取消，看板上显示IP
```

client：

```bash
nohup python ping.py &
```

server:

```bash
nohup python server.py &
```
