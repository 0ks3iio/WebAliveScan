# WebAliveScan
安装
```
pip3 install -r requirements.txt -i https://mirrors.aliyun.com/pypi/simple/
```

使用帮助：
```
python3 webscan.py --target target.txt --port 80
python3 webscan.py --target target.txt --port large
```

##### v1.1增加忽略指定HTTP状态
```
config.py

# 可以指定需要忽略HTTP状态码
ignore_status_code = [400]

# 指定线程数量
threads = 1024
```


##### v1.2增加单个目标自定义端口
```
target.txt

# 根据--port指定的端口来扫描
www.google.com

# 只会扫描www.baidu.com的443端口
www.baidu.com:443
```
