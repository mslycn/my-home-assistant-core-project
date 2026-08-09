


## ha-mcp、ha-mcp-integration 和 Home Assistant 官方 MCP Server 三者的详细对比图（包括工具数量、能力范围、适用场景）

| 功能              |  官方 MCP Server | HA MCP Server（Integration） |   ha-mcp Docker   |
| --------------- | :------------: | :------------------------: | :---------------: |
| 控制设备            |        ✅       |              ✅             |         ✅         |
| 查询 Entity       |        ✅       |              ✅             |         ✅         |
| 所有 Entity       | ❌ Assist 暴露的实体 |              ✅             |         ✅         |
| 创建 Automation   |        ❌       |              ✅             |         ✅         |
| 修改 Automation   |        ❌       |              ✅             |         ✅         |
| 调试 Automation   |        ❌       |              ✅             |         ✅         |
| Dashboard       |        ❌       |              ✅             |         ✅         |
| History         |       基础       |              ✅             |         ✅         |
| Trace           |        ❌       |              ✅             |         ✅         |
| Helpers         |        ❌       |              ✅             |         ✅         |
| HACS            |        ❌       |              ✅             |         ✅         |
| Add-ons         |        ❌       |              ✅             |         ✅         |
| File/YAML Tools |        ❌       |            ✅（可选）           | ✅（配合 Integration） |
