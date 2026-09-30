# LegacyIsland

LegacyIsland 是 ClassIsland 1.3 以前版本的历史归档 Fork，用于保存因 Microsoft Visual Studio App Center 关停而丢失的早期发布包与对应代码历史。

本仓库的 `master` 以 ClassIsland `1.2.2.0` 发布提交为代码基线。它是一个冻结的历史归档，不代表 ClassIsland 当前开发主线，也不承诺现代插件、在线服务或新系统兼容性维护。

## 归档内容

仓库保留以下历史版本及其 Git tag：

- [1.0](https://github.com/unDefFtr/LegacyIsland/releases/tag/1.0)
- [1.0.0.1](https://github.com/unDefFtr/LegacyIsland/releases/tag/1.0.0.1)
- [1.0.0.2](https://github.com/unDefFtr/LegacyIsland/releases/tag/1.0.0.2)
- [1.0.3](https://github.com/unDefFtr/LegacyIsland/releases/tag/1.0.3)
- [1.1.0](https://github.com/unDefFtr/LegacyIsland/releases/tag/1.1.0)
- [1.2.0.0](https://github.com/unDefFtr/LegacyIsland/releases/tag/1.2.0.0)
- [1.2.2.0](https://github.com/unDefFtr/LegacyIsland/releases/tag/1.2.2.0)

`1.2.2.0` 是本归档的最新基线。每个 Release 都包含对应的 Windows x64 构建压缩包。

早期的独立历史线保存在 [`archive/archaeology-2023`](https://github.com/unDefFtr/LegacyIsland/tree/archive/archaeology-2023) 分支中。

## 构建

`master` 基线使用 .NET 8、WPF 和 Windows 桌面目标。请在 Windows 环境安装 .NET 8 SDK 后执行：

```powershell
dotnet build ClassIsland.sln -c Release
```

如需生成 Windows x64 发布目录：

```powershell
dotnet publish .\ClassIsland\ClassIsland.csproj `
  -c Release `
  -r win-x64 `
  --self-contained true
```

仓库中的 GitHub Actions workflow 可用于历史版本构建；手动触发时应将 `release_tag` 指向目标版本 tag。

## 项目来源

LegacyIsland 源自 [ClassIsland/ClassIsland](https://github.com/ClassIsland/ClassIsland)。当前版本的项目文档、社区信息与开发活动请以原项目为准：

- [ClassIsland](https://github.com/ClassIsland/ClassIsland)
- [ClassIsland Releases](https://github.com/ClassIsland/ClassIsland/releases)

## 许可协议

请参阅仓库中的 [LICENSE.txt](LICENSE.txt)。
