# GitHub Codespaces 使用指南

## 一、概述
GitHub Codespaces 是一个基于云端的开发环境，允许开发者在浏览器或 Visual Studio Code 中直接编写、测试和调试代码，无需在本地设置复杂的开发环境。它自带了 Python、Node.js 及 Docker 环境，并提供每月 120 小时的免费使用时长。

## 二、优势
- **无需本地配置**：无需在本地安装复杂的开发工具和依赖环境，直接在云端开始开发。
- **多语言支持**：内置 Python、Node.js 等常用开发环境，支持多种编程语言。
- **与 VS Code 无缝集成**：支持在浏览器中直接使用 VS Code 的功能，也可以将 Codespace 连接到本地的 VS Code。
- **Docker 部署**：内置 Docker 与 Docker Compose，可部署任意docker镜像。
- **高网速高性能**：2核4G或4核8G可选。
- **高网速高性能**：2核4G或4核8G可选。
- **免费时长**：每月提供 120 小时的免费使用时长，满足日常开发需求。

## 三、设置与使用

### （一）创建 Codespace
1. **登录 GitHub**：访问 [GitHub 官网](https://github.com/) 并登录你的账号。
2. **选择仓库**：进入你想要开发的仓库。
3. **创建 Codespace**：
   - 点击右上角的 `Code` 按钮，选择 `Codespaces`。
   - 点击 `New codespace`，选择合适的机器配置（默认配置通常足够）。
   - 点击 `Create`，等待 Codespace 初始化完成。

### （二）使用内置环境
- **Python 环境**：Codespace 自带 Python 环境，可以直接运行 Python 脚本。
  ```bash
  python --version
  ```
- **Node.js 环境**：支持 Node.js 开发，可以直接运行 Node.js 项目。
  ```bash
  node --version
  npm --version
  ```
- **Docker 环境**：支持 Docker 容器化开发。
  ```bash
  docker --version
  ```

### （三）通过 Docker 部署 KasmWeb 虚拟浏览器
1. **拉取 KasmWeb 镜像**：
   ```bash
   docker pull kasmtech/kasm_workspaces:latest
   ```
2. **运行 KasmWeb 容器**：
   ```bash
   docker run -d -p 80:80 kasmtech/kasm_workspaces
   ```
3. **访问 KasmWeb**：
   - 在浏览器中访问 `http://localhost`（如果在本地运行）或对应的 Codespace 端口转发地址。
   - 通过 KasmWeb 的虚拟浏览器访问国外站点。

## 四、注意事项
- **资源限制**：虽然每月有 120 小时的免费时长，但长时间运行可能会消耗较多资源，请合理使用。
- **网络访问**：使用 KasmWeb 虚拟浏览器访问国外站点时，需确保网络环境稳定。
- **数据安全**：不要在 Codespace 中存储敏感数据，定期清理不必要的文件和数据。

## 五、常见问题
### Q1：如何连接本地 VS Code 到 Codespace？
- 打开 VS Code，点击左侧的 `Remote Explorer`。
- 选择 `GitHub Codespaces`，找到你的 Codespace，点击 `Connect`。

### Q2：如何停止或删除 Codespace？
- 在 GitHub 的 `Codespaces` 页面，找到对应的 Codespace。
- 点击 `Actions`，选择 `Stop` 停止运行，或选择 `Delete` 删除 Codespace。

## 六、总结
GitHub Codespaces 提供了一个强大且便捷的云端开发环境，适合快速开发和测试项目。通过 Docker 部署 KasmWeb 虚拟浏览器，还可以实现对国外站点的访问，进一步扩展了其应用场景。希望本文能帮助你更地使用 GitHub Codespaces。

<!--stackedit_data:
eyJoaXN0b3J5IjpbNDc0NTk3ODY0LC0xMTQ3OTg1ODI1LDEwMz
Q0NDM4NjRdfQ==
-->