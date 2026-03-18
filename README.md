# BSDCN Hexo 主题

一个受 FreeBSD 官方网站设计启发的 Hexo 主题。

## 特性

- **视觉设计**：复刻 FreeBSD 官网简洁、专业的外观
- **响应式布局**：适配不同屏幕尺寸（手机、平板、桌面）
- **导航结构**：包含主导航、语言选择器和页脚链接
- **内容分区**：分为新闻、活动、媒体报道、安全公告和勘误通知等部分
- **可定制**：通过 `_config.yml` 轻松配置

## 安装

1. 将主题克隆到你的 Hexo 站点的 `themes` 目录：

```bash
git clone https://github.com/yourusername/hexo-theme-bsdcn.git themes/bsdcn
```

2. 更新你的 Hexo 站点的 `_config.yml` 以使用该主题：

```yaml
theme: bsdcn
```

3. 安装依赖（如果有）：

```bash
npm install
```

## 配置

编辑 `themes/bsdcn/_config.yml` 文件来自定义主题：

### 站点设置
```yaml
site:
  title: FreeBSD
  subtitle: The Power to Serve
  description: FreeBSD 是一个用于驱动现代服务器、桌面和嵌入式平台的操作系统。
  logo: /images/freebsd-logo.png
```

### 导航
```yaml
nav:
  items:
    - text: 首页
      link: /
    - text: 关于
      link: /about/
    - text: 下载
      link: /download/
    - text: 文档
      link: /documentation/
    - text: 社区
      link: /community/
```

### 语言
```yaml
language:
  default: en
  available:
    - en
    - ru
    - zh-tw
```

### 主题颜色
```yaml
theme:
  primary_color: #003366
  secondary_color: #0066cc
  text_color: #333333
  background_color: #ffffff
  border_color: #dddddd
```

## 文件结构

```
hexo-theme-bsdcn/
├── _config.yml          # 主题配置
├── layout/
│   └── layout.ejs       # 主布局模板
├── source/
│   ├── css/
│   │   └── style.css    # 主样式表
│   ├── js/
│   │   └── main.js      # JavaScript 功能
│   └── images/          # 图片文件
└── README.md            # 主题文档
```

## 开发

要修改主题：

1. 在 `layout` 目录中编辑 EJS 模板
2. 在 `source/css/style.css` 中更新样式
3. 在 `source/js/main.js` 中添加自定义 JavaScript
4. 将图片添加到 `source/images/`

## 许可证

MIT 许可证

## 致谢

受 [FreeBSD 官方网站](https://www.freebsd.org/) 启发
