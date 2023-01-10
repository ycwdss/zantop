# 从 VitePress 0.x 迁移

如果您来自 VitePress 0.x 版本，由于新功能和增强功能，会有一些重大更改。 请按照本指南了解如何将您的应用程序迁移到最新的 VitePress。

## App Config

- 国际化功能尚未实现。

## Theme Config

- `sidebar` 选项改变了它的结构。
   - `children` key现在命名为 `items`。
   - 顶级项目目前可能不包含“链接”。 我们打算把它转回来。
- 删除了`repo`、`repoLabel`、`docsDir`、`docsBranch`、`editLinks`、`editLinkText`，以支持更灵活的api。
   - 要将带有图标的 GitHub 链接添加到导航，请使用 [社交链接](./theme-nav#navigation-links) 功能。
   - 要添加“编辑此页面”功能，请使用 [编辑链接](./theme-edit-link) 功能。
- `lastUpdated` 选项现在分为 `config.lastUpdated` 和 `themeConfig.lastUpdatedText`。
- `carbonAds.carbon` 更改为 `carbonAds.code`。

## Frontmatter Config

- `home: true` 选项已更改为 `layout: home`。 此外，还修改了许多与主页相关的设置以提供附加功能。 详情请参阅 [主页指南](./theme-home-page)。
- `footer` 选项移至 [`themeConfig.footer`](../config/theme-configs#footer)。
