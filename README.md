# 宁夏交通厅互联网信息日报

## 文件

- `daily_report_linux_v2.tgz` (16.8MB) - Linux 自包含 v2, 含全网数据补充

## 部署

```bash
tar xzf daily_report_linux_v2.tgz
cd linux/
chmod +x run.sh daily_report
./run.sh
```

## 系统要求

- 任意 Linux 发行版 (glibc 2.36+)
- 不需要 Python / pip / 任何依赖
- 单文件二进制自包含

## 输出

`reports/互联网信息汇总YYYY.MM.DD.docx`

## 数据源

- 内网: 120.27.2.34:8081 宁夏交通运输行业互联网信息
- 外网: 今日头条移动版搜索 (28 个交通相关关键词)

## 规则

6 重点分类: 公交 / 出租 / 网约 / 客货 / 危化 / 司乘权益 / 公路

硬排除: 交通事故、交警相关、外省、官方通告、广告
