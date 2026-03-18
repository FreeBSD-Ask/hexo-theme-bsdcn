# BSDCN Theme for Hexo

A Hexo theme inspired by the FreeBSD official website design.

## Features

- **Visual Design**: Recreates the clean, professional look of the FreeBSD website
- **Responsive Layout**: Adapts to different screen sizes (mobile, tablet, desktop)
- **Navigation Structure**: Includes main navigation, language selector, and footer links
- **Content Sections**: Organized into news, events, press, security advisories, and errata notices
- **Customizable**: Easy to configure via `_config.yml`

## Installation

1. Clone the theme into your Hexo site's `themes` directory:

```bash
git clone https://github.com/yourusername/hexo-theme-bsdcn.git themes/bsdcn
```

2. Update your Hexo site's `_config.yml` to use the theme:

```yaml
theme: bsdcn
```

3. Install dependencies (if any):

```bash
npm install
```

## Configuration

Edit the `themes/bsdcn/_config.yml` file to customize the theme:

### Site Settings
```yaml
site:
  title: FreeBSD
  subtitle: The Power to Serve
  description: FreeBSD is an operating system used to power modern servers, desktops, and embedded platforms.
  logo: /images/freebsd-logo.png
```

### Navigation
```yaml
nav:
  items:
    - text: Home
      link: /
    - text: About
      link: /about/
    - text: Download
      link: /download/
    - text: Documentation
      link: /documentation/
    - text: Community
      link: /community/
```

### Language
```yaml
language:
  default: en
  available:
    - en
    - ru
    - zh-tw
```

### Theme Colors
```yaml
theme:
  primary_color: #003366
  secondary_color: #0066cc
  text_color: #333333
  background_color: #ffffff
  border_color: #dddddd
```

## File Structure

```
hexo-theme-bsdcn/
├── _config.yml          # Theme configuration
├── layout/
│   └── layout.ejs       # Main layout template
├── source/
│   ├── css/
│   │   └── style.css    # Main stylesheet
│   ├── js/
│   │   └── main.js      # JavaScript functionality
│   └── images/          # Image files
└── README.md            # Theme documentation
```

## Development

To modify the theme:

1. Edit the EJS templates in the `layout` directory
2. Update the styles in `source/css/style.css`
3. Add custom JavaScript in `source/js/main.js`
4. Add images to `source/images/`

## License

MIT License

## Credits

Inspired by the [FreeBSD official website](https://www.freebsd.org/)