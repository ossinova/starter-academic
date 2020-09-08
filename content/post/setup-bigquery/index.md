---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Setup Bigquery"
subtitle: "A quick guide on how to setup BigQuety"
summary: "Instruction on how to setup BigQuery"
authors: [Oscar Dyremyhr]
tags: [bigquey, data, cloud]
categories: [clud, bigquery]
date: 2020-09-04T14:44:26+02:00
lastmod: 2020-09-04T14:44:26+02:00
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

# Setup

Setting up BigQuery takes a few minutes. Go to your console.cloud.google.com page and add the BigQuery service to your project.


![alt text](\images\setup-bigquery.PNG "BigQuery")

Click on create dataset and fill in the information as you wish. Once complete we can add tables and propagate it with data. If you wish to upload a CSV file you would need to eanable the BigQuery API.

You can also use one of the free public datasets by running a SQL statement and saving the result to a table.

```sql
SELECT
  name, gender,
  SUM(number) AS total
FROM
  `bigquery-public-data.usa_names.usa_1910_2013`
GROUP BY
  name, gender
ORDER BY
  total DESC
LIMIT
  10

```
