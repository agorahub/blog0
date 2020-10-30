---
layout: page
title:  BLOG⓪
permalink: /readme/
comments_repo: agorahub/blog0
comments_id: 1
---

Read blogs on demand.

| Source  | Importer   | Update |
| ------  | --------   | ------ |
| INITIUM | RSSINITIUM | Daily  |
| MATTERS | RSSMATTERS | Daily  |
| VOCUS   | RSSVOCUS   | Daily  |


## Import and Commit

```
# Customize RSS importers in local gem 'jekyll-import':
$ ls .../gems/jekyll-import-{version}/lib/jekyll-import/importers/rss*
# rssinitium.rb rssmatters.rb rssvocus.rb

# Import RSS feeds and commit posts back:
$ ./_feed.sh  # pull, import, archive, add, commit, push
```

## Batch and Automate

[Check comment](https://github.com/agorahub/news0/issues/1#issuecomment-597540617)

## Test and Deploy

```
# Edit _config.yml for local bundle test:
$ gem install bundler jekyll
$ bundle exec jekyll serve
# => Now browse to http://localhost:4000

# Edit _config.yml for production bundle:
$ JEKYLL_ENV=production bundle exec jekyll build
# Copy the compiled codes from _site/ to your html server.
```

{% include comments.html %}

## Disclaimer

The information and opinions within this website are for information purposes only. They are not intended to constitute legal or other professional advice, and should not be relied on or treated as a substitute for specific advice relevant to particular circumstances. We accept no responsibility for any errors, omissions or misleading statements on this website, or for any loss which may arise from reliance on materials contained on this website. Certain parts of this site may link to external Internet sites, and other external Internet sites may link to this website. We are not responsible for the content of any external Internet sites.

