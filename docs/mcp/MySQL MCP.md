# 目的
* 了解如何在Trae中配置MySQL MCP
* 了解如何在Trae中使用MySQL MCP

# 请先阅读
* [MCP基础知识](MCP基础知识.md)

# 方法
### 配置
```JSON
{
  "mcpServers": {
    "mysql": {
      "command": "uv",
      "args": [
        "run",
        "mysql_mcp_server"
      ],
      "env": {
        "MYSQL_HOST": "localhost",
        "MYSQL_PORT": "3306",
        "MYSQL_USER": "<user_name>",
        "MYSQL_PASSWORD": "<user_pwd>",
        "MYSQL_DATABASE": "<default_db>"
      }
    }
  }
}
```
### 元数据查询


# 总结
列出相关的总结内容，尤其是有助于将方法转化为知识的总结。

# 参考资料
* [github:mysql_mcp_server](https://github.com/designcomputer/mysql_mcp_server)



