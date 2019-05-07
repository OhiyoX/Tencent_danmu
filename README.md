

# 腾讯弹幕抓取器

首先我们来看一下它是怎么工作的吧.

![useage.gif](.//media/useage.gif)


## Feature

- 异步任务抓取
- 任意视频弹幕抓取
- 可定制单集时长
- XLSX生成
- 词云生成
- json生成

## 环境安装

我们通过如下命令克隆代码仓库到本地并通过pipenv安装依赖环境

```
git clone git@github.com:aoii103/Tencent_danmu.git
cd Tencent_danmu
pipenv install
```


## 基础运行

```
python main.py -u [url]
```

## 命令参数

```
Usage: main.py [OPTIONS]

Options:
  -u, --url TEXT          指定目标URL
  -t, --max_time INTEGER  指定每集时间长度，不宜过大(针对vip视频)
  -v, --vip               vip默认设置15000秒
  -c, --cons INTEGER      爬行并发数量
  -n, --new               不使用缓存生成
  -e, --excel             是否生成Excel
  -w, --words             是否生成词云
  -g, --graph             是否生成分析图(未做)
  --help                  Show this message and exit.

```


## TODO

- 基础图形生成
- 其他功能