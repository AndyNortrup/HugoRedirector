This is a very simple project that I spun up to show that if you were looking to have custom url shortener with out scheevy ad-tech, you could do that with Hugo.  This could effectively be hosted for free on GitHub Pages and you could add new pages with a single markdown file.

## Setup
1. Create a repository
2. Setup your [custom domain](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site) (something short if you want a shortened link)
3. Configure Github Actions to [build pages on update](https://gohugo.io/hosting-and-deployment/hosting-on-github/).

Add a new file to `/layouts/page/<file>.md`

Fill in these fields in the front matter:
```
---
layout: redirector
title: Nortrup in Development
target: http://www.nortrup.dev
---

```

Build and depoly and you can shorten your own urls.