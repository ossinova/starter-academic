---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Dashboards using Google DataStudio and BigQuery"
subtitle: "An introduction to DataStudio"
summary: "A tutorial on how to use DataStudio and BigQuery to create beautiful dashboards"
authors: [Oscar Dyremyhr]
tags: [bigquery, data, visualization, datastudio]
categories: [visualization, cloud]
date: 2020-09-04T13:53:34+02:00
lastmod: 2020-09-04T13:53:34+02:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

# Getting Started

DataStudio is a very cool and suprisingly user-friendly tool built by Google. It allows for the creation of Dashboards and visualization by connecting a data source such as a CSV file or a database. In this tutorial we will be using BigQuery, another Google product that works very nicely in conjuntion with DataStudio.

Head over to [DataStudio] and log in with your Google account.

You should see something like this:

<iframe width="600" height="800" src="https://datastudio.google.com/embed/reporting/31e8b262-2d18-48a9-8483-d0a3b9ed7abf/page/1M" frameborder="0" style="border:0" allowfullscreen></iframe>




# Connecting to BigQuery

Once you have created a DataStudio project you can connect a data source. Fr the purpose of this tutorial we will be using BigQuery. You can connect to BigQuery, by selecting it:





If you do not a BigQuery instance. I have a blog post that goes through how you can set up one [here][SetupBigQuery]










[DataStudio]: https://datastudio.google.com/
[SetupBigQuery]: https://ossinova.me/post/setup-bigquery/
