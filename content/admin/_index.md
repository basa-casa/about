---
title: Admin
CMS: https://unpkg.com/@sveltia/cms/dist/sveltia-cms.js
collections:
  - import: collection admin-hugo-pages
    collection_type: import
  - import: collection about
    collection_type: import
  - import: collection content-sections
    collection_type: import
    extend: null
  - import: collection hugo-content-default
    collection_type: import
    extend:
      name: blog
      label: Blog
      description: "Blog posts for Basa Casa"
      folder: content/blog
      identifier_field: title
draft: false
menus:
  - admin
  - adminHelp
cascade:
  cms: https://unpkg.com/@sveltia/cms/dist/sveltia-cms.js
  outputs:
    - HTML
    - scms_config
    - help
  config:
    backend:
      branch: main
      name: github
      repo: basa-casa/admin
    media_folder: assets/img
    public_folder: img
    site_url: ../../
    display_url: /
    logo_url: /img/admin.png
---
Welcome to `/admin/help`!
