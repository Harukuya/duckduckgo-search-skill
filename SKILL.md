---
name: duckduckgo-search
description: 使用 DuckDuckGo 进行免费网页搜索，无需 API key。当用户需要搜索实时信息、新闻、图片或网页时使用此 skill。支持中文搜索。
---

# DuckDuckGo Search

使用免费的 DuckDuckGo 搜索工具获取实时信息。

## 工具

使用 Python + `ddgs` 包进行搜索：

```python
from ddgs import DDGS

def search(query, max_results=30):
    ddgs = DDGS()
    results = ddgs.text(query, max_results=max_results)
    return results
```

## 使用方式

当用户要求搜索时，执行以下步骤：

1. **安装依赖**（如未安装）：
   ```bash
   pip install ddgs
   ```

2. **执行搜索**并返回结果

## 示例

搜索 "今日新闻"（默认返回30条）：
- 返回标题、链接和摘要

## 注意

- 这是免费的，无需 API key
- 有速率限制，避免频繁大量请求
- 适合实时信息、新闻、快速查询
