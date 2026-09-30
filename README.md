# LegacyIsland

LegacyIsland 是 ClassIsland 早期版本的历史归档 Fork，保留 1.3 以前的代码、版本标签与 Windows 构建产物。

本仓库不代表 ClassIsland 当前开发主线，也不承诺为现代系统、插件或在线服务提供兼容性维护。

## 版本范围

仓库包含以下历史版本：

- [1.0](https://github.com/unDefFtr/LegacyIsland/releases/tag/1.0)
- [1.0.0.1](https://github.com/unDefFtr/LegacyIsland/releases/tag/1.0.0.1)
- [1.0.0.2](https://github.com/unDefFtr/LegacyIsland/releases/tag/1.0.0.2)
- [1.0.3](https://github.com/unDefFtr/LegacyIsland/releases/tag/1.0.3)
- [1.1.0](https://github.com/unDefFtr/LegacyIsland/releases/tag/1.1.0)
- [1.2.0.0](https://github.com/unDefFtr/LegacyIsland/releases/tag/1.2.0.0)
- [1.2.2.0](https://github.com/unDefFtr/LegacyIsland/releases/tag/1.2.2.0)

`1.2.2.0` 是本归档中 1.3 以前的最后一个版本。每个版本均对应一个 Git tag，并提供 Windows x64 构建压缩包。

## 构建

历史代码使用 .NET 6 和 WPF，构建目标为 Windows x64。

```powershell
msbuild .\ClassIsland\ClassIsland.csproj `
  /restore `
  /t:Publish `
  /p:Configuration=Release `
  /p:PublishProfile=FolderProfile
```

构建结果位于：

```text
ClassIsland/bin/Release/net6.0-windows/publish/win-x64
```

GitHub Actions workflow 支持通过 `workflow_dispatch` 指定历史 tag：

- `ref`：要构建的版本 tag
- `version`：构建产物使用的版本号

## 项目来源

LegacyIsland 源自 [ClassIsland/ClassIsland](https://github.com/ClassIsland/ClassIsland)。当前版本的项目文档、社区信息与开发活动请以原项目为准：

- [ClassIsland](https://github.com/ClassIsland/ClassIsland)
- [ClassIsland Releases](https://github.com/ClassIsland/ClassIsland/releases)

## 许可协议

请参阅仓库中的 [LICENSE.txt](LICENSE.txt)。
