# Carbon Ads

VitePress内置了对 [Carbon Ads](https://www.carbonads.net/) 的原生支持。通过在配置中定义Carbon Ads凭证，VitePress将在页面上显示广告。

```js
export default {
  themeConfig: {
    carbonAds: {
      code: 'your-carbon-code',
      placement: 'your-carbon-placement'
    }
  }
}
```

这些值用于调用 carbon CDN 脚本，如下所示。

```js
`//cdn.carbonads.com/carbon.js?serve=${code}&placement=${placement}`
```

如需了解有关 Carbon Ads 配置的更多信息，请访问 [Carbon Ads website](https://www.carbonads.net/)。
