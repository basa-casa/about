---
title: "The creation of basa-casa/admin"
# meta title
meta_title: "The Admin static site CMS generator"
# meta description
description: "The hugo modules github.com/basa-casa/admin, admin-scms, and admin-hugo allow static site builders, owners, and maintainers, to quickly build complex CMS solutions to their git-stored text files."
date: 2024-09-27T05:00:00Z
# image: "/images/admin.png"
categories: ["/admin"]
author: "Brian MacKinney"
draft: false
---

## A Module Story

One day I discovered NetlifyCMS. I needed something like it at the time, and when configuring it stumbled across the New Dynamic's module for splitting config files with a simple import function during a hugo build. It worked great, and I started creating a CMS that made the CMS, collection, and field files. 

{{< image src="images/nc-admin.png" caption="" alt="alter-text" height="" width="" position="center" command="fill" option="q100" class="img-fluid" title="image title"  webp="false" >}}

### Then NetlifyCMS died

You might have seen me a few years ago, while working on this module, get frustrated and [ask Netlify if their CMS was dead](https://answers.netlify.com/t/is-this-project-dead/70988). I'd just about wrapped up the first edition, pointing a set of templates and collection and field files at NetlifyCMS config files. RIP NetlifyCMS. 

### Then there was hugo-admin

{{< image src="images/hugo-scms-admin.png" caption="" alt="alter-text" height="" width="" position="center" command="fill" option="q100" class="img-fluid" title="image title"  webp="false" >}}

Then I added hugo configuration fields and collections, and made the mistake of adding content in the module. Both people who installed the module get 5 CMS pages added to their sites. I stop making sites, and nothing much happens. The module does gain 15 stars on GitHub, though! In this era, we relied on StaticJsCMS for the javascript and proxy server. Unfortunately it died right before I actually had a use for all of it. RIP.

### Now we have admin, admin-scms, and admin-hugo

{{< image src="images/admin.png" caption="" alt="alter-text" height="" width="" position="center" command="fill" option="q100" class="img-fluid" title="image title"  webp="false" >}}

Sveltia-CMS exists and saves the day for now! It looks better, seems to be a simpler solution, edits local files without running a second server, and the maintainer is SUPER responsive and seems pretty capable at fixing bugs. I used the discovery to prompt me to split the module into separate modules for each set of collections and fields. Admin has the layouts and can import collections into the admin CMS. admin-scms has examplesite pages for CMS control of collections and fields, and all of the collection and fields yaml files needed to construct them. Admin-hugo has all of this for hugo configuration, content, and data.

## An opportunity to use it

I have the great fortune to be in a position at one of the world's largest tech companies, where I'm going to use /admin on a small project with a fairly high profile. When I started there I created collections and fields for our training content. They haven't been necessary yet, but will be soon. I'm grateful to Sveltia-CMS maintainer 
