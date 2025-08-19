# SEO Checker

一个基于PyQt6和httpx的现代化SEO检测工具，可以批量检查网站的标题、关键词、描述，并检测网页篡改情况。

## 功能特性

- 批量检测网站SEO信息（标题、关键词、描述）
- 支持多种User-Agent（桌面、移动、爬虫）
- 关键词库匹配检测
- 网页篡改检测（比较不同UA的响应内容）
- 高并发处理（可调节并发数）
- 结果导出（CSV/JSON格式）
- 自定义关键词库

## 安装依赖

```bash
pip install -r requirements.txt
```

## 使用说明

1. 运行程序：
```bash
python run.py
```

2. 在输入框中输入要检测的URL（每行一个）
3. 点击"开始检测"按钮
4. 查看检测结果

## 配置选项

- 设置最大并发数
- 选择User-Agent类型
- 编辑关键词库

## 截图
主界面
https://raw.githubusercontent.com/govbk/SEO-Check/refs/heads/main/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_2025-08-19_125027_481.png
自定义规则库
https://raw.githubusercontent.com/govbk/SEO-Check/refs/heads/main/wechat_2025-08-19_124945_036.png
自定义UA
https://raw.githubusercontent.com/govbk/SEO-Check/refs/heads/main/wechat_2025-08-19_124925_013.png

## 许可证

MIT
