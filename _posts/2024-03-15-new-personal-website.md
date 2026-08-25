---
title: "My New Personal Website"
categories:
  - Blog
tags:
  - GitHub Pages
  - Minimal Mistakes
  - Meta
---

Welcome to my new personal website! I've once again decided to rebuild this site which has gone through a few different iterations now, originally hosted on a Pi3 and later migrated to GitHub Pages for simplified hosting. The previous iteration can be seen [in my old repo here](https://github.com/alexwaibel/alexwaibel.github.io-indigo-archive).

This time around I've gone with a simplified setup using the [Minimal Mistakes template repo](https://github.com/mmistakes/mm-github-pages-starter). My hope is that by migrating to this template I can merge in any upkeep tasks and changes from that template and focus primarily on content rather than churn maintaining the site itself. GitHub Pages has proved very reliable in the past for hosting simple sites like this.

Publishing new articles is extremely easy with this setup. All you need to do is create a new Markdown document in the `_posts` directory. When it is pushed, a GitHub Actions [workflow](https://github.com/{{site.repository}}/blob/master/.github/workflows/jekyll.yml) automatically deploys it. For example, see the [source for this article](https://github.com/{{site.repository}}/blob/master/_posts/2024-03-15-new-personal-website.md).

If you're interested in hosting a similar website yourself it's quite easy. Check out the [GitHub Pages docs](https://pages.github.com/) for a quick start. There's a ton of available open source templates to get you started or you can create a Jekyll site yourself from scratch.

I'm hoping to publish more posts this time around, especially as I rebuild my home server and network and dive deeper into cybersecurity topics. If you want to subscribe for future updates, the site is also published as an RSS feed [here]({{ site.url }}/feed.xml).
