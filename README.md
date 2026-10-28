# pawnPromotion Blog

Personal blog rebuilt with Hexo and Fluid.

## Local Commands

```bash
npm.cmd install
npm.cmd run build
npm.cmd run server
```

Local preview defaults to:

```text
http://localhost:4000
```

## Write Posts

Posts live in:

```text
source/_posts/
```

Create a new post:

```bash
npx hexo new "文章标题"
```

Images should be placed in:

```text
source/img/
```

Use images in Markdown:

```md
![图片说明](/img/example.jpg)
```

## Main Files To Edit

- `_config.yml`: site title, author, URL, permalink and Hexo options.
- `_config.fluid.yml`: Fluid theme options, navbar, homepage banner, about page profile.
- `source/_posts/`: blog posts.
- `source/about/index.md`: about page content.
- `source/projects/index.md`: portfolio page content.
- `source/img/avatar.svg`: avatar placeholder.
- `source/img/banner.svg`: homepage and post banner placeholder.

## Deploy

The site deploys through GitHub Actions. Keep GitHub repository settings as:

```text
Settings -> Pages -> Build and deployment -> Source -> GitHub Actions
```

Push to `main`; the workflow builds Hexo and uploads the generated `public/` directory to GitHub Pages.
