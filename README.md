# easyconnect-docker-cli

<!-- starswhere-docs-overview -->

## 项目概览

**定位**：一个用于管理 EasyConnect 容器化运行的轻量配置仓库。

**核心功能**：
- 提供 Docker Compose 编排文件
- 包含开发环境变量模板
- 适合把 EasyConnect 放入容器中统一启动
- 仓库结构简单，便于按本机网络环境改造

**技术栈**：Docker Compose、环境变量配置。

**目录与模块**：`docker-compose.yml` 是核心编排文件；`.env.development` 保存开发环境参数示例。

**使用方式**：根据 `.env.development` 调整本地参数后，通过 Docker Compose 管理容器。

**配置说明**：所有关键运行参数应写入环境变量文件或 compose，避免硬编码到镜像。

**适用场景**：适合需要容器化 EasyConnect 客户端或相关网络环境的场景。

**注意事项**：VPN/网络类容器通常依赖宿主机权限、网络模式和路由策略，部署前需要按平台确认。

<!-- /starswhere-docs-overview -->

