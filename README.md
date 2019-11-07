
### 说明
本项目是基于"为知笔记"构建的一个本地搜索引擎, 可以认为是 "为知笔记" + "百度搜索" 的综合效果
可以实时解析笔记本本机的为知笔记数据, 分钟级别自动更新到搜索引擎中
```
这套搜索引擎的基本特性是:
[1] 目前仅支持 Mac 平台, 主要用 shell + python实现
[2] 自动解析搜索笔记本本地数据
[3] 使用浏览器 web 页面做为搜索入口
[3] 支持 query 和文本切词
[4] 基本原理是使用倒排索引 和 检索拉链归并
[5] 排序算法支持 TF*IDF, term 紧密度, 标题提权
[6] 支持 markdown 格式自动渲染
[7] 支持 减法语法查询
[8] 支持摘要自动提取和关键词飘红
[9] 自动适应新增的笔记和删除的笔记(1分钟延迟)
```

### 为知笔记官网
http://www.wiz.cn/zh-cn

### Install 安装
[1] 先从为知笔记官网下载mac 版客户端, 登录自己的账户, 创建笔记
[2] 下载本工具到mac笔记本任意目录, 然后执行:
    bash start.sh
    Wait for 2min for success

### Error log 
cat error.log

### Search
open http://127.0.0.1:9009 on your chrome or safair

### Change Listen Port
bash change_to_port.sh 8080
