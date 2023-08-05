# shariff.dev

Source code for my personal website.

# Run on local machine

## Install hugo

[https://gohugo.io/getting-started/installing/](https://gohugo.io/getting-started/installing/)

## Clone the repo

```sh
git clone https://github.com/itsyaasir/shariff.dev.git
```

```sh
cd shariff.dev


```

## Install theme (e.g. PaperMod)

```sh
git clone https://github.com/adityatelange/hugo-PaperMod themes/PaperMod
git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
```

## Run

```sh
hugo server -D
```

Visit [localhost:1313](http://localhost:1313)

## To enable the comment

Open below file

```sh
vim themes/PaperMod/layouts/partials/comments.html
```

Add below snippet

```html
<script
  src="https://giscus.app/client.js"
  data-repo="itsyaasir/shariff.dev"
  data-repo-id="R_kgDOKDQ0NA"
  data-category="Announcements"
  data-category-id="DIC_kwDOKDQ0NM4CYXg6"
  data-mapping="pathname"
  data-strict="0"
  data-reactions-enabled="1"
  data-emit-metadata="0"
  data-input-position="top"
  data-theme="preferred_color_scheme"
  data-lang="en"
  data-loading="lazy"
  crossorigin="anonymous"
  async
></script>
```

## Add Cover page customization

Create below file

```sh
vim themes/PaperMod/assets/css/extended/tag_list_cover.css 
```

Add below CSS

```
.tag-entry .entry-cover {
    display: flex;
}
```

Re Generate the Site

```
hugo
```
