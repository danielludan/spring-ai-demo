# 目的
* 了解如何在Trae中配置MySQL MCP
* 了解如何在Trae中使用MySQL MCP

# 请先阅读
* [MCP基础知识](MCP基础知识.md)

# 方法
### MCP服务配置
1. 手动安装mysql-mcp-server包
```bash
pip install mysql-mcp-server
```
其实尝试过用uv --install命令能够自动安装但没有成功，所以只能手动安装。

2. 添加MySQL MCP服务配置。以下以STDIO方式启动
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
3. 创建新的智能体，选择“mysql”MCP服务

### 元数据查询

# 任务
- [ ] 不需要手动安装mysql-mcp-server包，使得uv在发现mysql_mcp_server不能启动时，能自动安装mysql-mcp-server包。

# 总结
列出相关的总结内容，尤其是有助于将方法转化为知识的总结。

# 参考资料
* [github:mysql_mcp_server](https://github.com/designcomputer/mysql_mcp_server)



