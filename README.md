# TongXiao Common Search MCP Server

A Model Context Protocol (MCP) server implementation that integrates with IQS APIs, which delivers clean, accurate, diverse, and high-quality results through multiple data sources.
For more Information about TongXiao, please visit our [documents](https://help.aliyun.com/product/2837261.html?spm=5176.29875775.0.0.15362064NYv3s0).

<a href="https://glama.ai/mcp/servers/@aliyun/alibabacloud-iqs-tongxiao-mcp-server">
  <img width="380" height="200" src="https://glama.ai/mcp/servers/@aliyun/alibabacloud-iqs-tongxiao-mcp-server/badge" alt="TongXiao Common Search Server MCP server" />
</a>

## Installation

### NPM Installation
```bash
npm install -g @tongxiao/common-search-mcp-server
```

### Running with npx
```bash
# run stdio server
env TONGXIAO_API_KEY=your-api-key npx -y @tongxiao/common-search-mcp-server
```
```bash
# run sse server
env TONGXIAO_API_KEY=your-api-key SERVER=sse npx -y @tongxiao/common-search-mcp-server
```


You can find your apikey from [ipaas.console.aliyun.com/api-key](https://ipaas.console.aliyun.com/api-key)

### Running on client
Configure Tongxiao MCP Server directly on mainstream MCP Client.

```json
{
    "mcpServers": {
        "tongxiao-common-search": {
            "command": "npx",
            "args": [
                "-y",
                "@tongxiao/common-search-mcp-server"
            ],
            "env": {
                "TONGXIAO_API_KEY": ""
            }
        }
    }
}
```

## Available Tools
1. common_search
This tool offers enhanced real-time search capabilities for open domain networks. By utilizing optimization with large models and integrating multiple data sources, it delivers clean, accurate, diverse, and high-quality results.

**Best for:**
When you are unsure where to find information, use this interface to obtain accurate information from the web or multiple vertical data sources.