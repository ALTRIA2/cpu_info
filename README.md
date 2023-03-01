# cpu_info
Linux查看CPU信息

## 查看cpu配置
```sh
cat /proc/cpuinfo
```

## 查看物理cpu个数
```sh
grep 'physical id' /proc/cpuinfo | sort -u
```
## 查看核心数量
```sh
grep 'core id' /proc/cpuinfo | sort -u | wc -l
```
## 查看线程数
```sh
grep 'processor' /proc/cpuinfo | sort -u | wc -l
```
