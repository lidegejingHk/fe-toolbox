# 网页应用 `<head>` 管理库

## [unhead](https://unhead.unjs.io/docs/typescript/head/guides/get-started/overview)

### 简介
Unhead 是一个功能强大、轻量且与框架无关的网页应用 head 管理库。
它允许你动态控制 HTML 文档的 <head> 元素，从而在任何 JavaScript 框架中提升 SEO、性能和用户体验。

### DEMO

```js
// use
useHead({
  title: 'Subscribe now!',
  htmlAttrs: {
    class: { dark: true, light: false }
  },
  bodyAttrs: {
    'style': { overflow: 'hidden' },
    'data-modal': true,
  },
  link: [{
    rel: 'preload',
    href: 'https://3p.com/subscribe.js',
    as: 'script',
  }],
})
```

```html
<!DOCTYPE html>
<html class="dark">
  <head>
    <title>Subscribe now!</title>
    <link rel="preload"
        href="https://3p.com/subscribe.js"
        as="script">
  </head>
  <body style="overflow: hidden;"
    data-modal>
  <!-- Your app -->
  </body>
</html>
```
