---
publish: true
created: <% tp.date.now('YYYY-MM-DD HH:mm') %>
modified: 2026-09-04T09:12:03.681Z
published: <% tp.date.now('YYYY-MM-DD HH:mm') %>
category:
  - work
  - data
  - research
date: <% tp.date.now('YYYY-MM-DD HH:mm') %>
reviewed: false
rating:
temporary: true
AI: false
---

Let’s break down when to use each method.

Start with Ordinary Least Squares (OLS) when you have more samples than features in your dataset, and when your features don’t strongly predict each other.

Ridge Regression works well when you have the opposite situation — lots of features compared to your number of samples. It’s also great when your features are strongly connected to each other.

Lasso Regression is best when you want to discover which features actually matter for your predictions. It will automatically set unimportant features to zero, making your model simpler.

Elastic Net combines the strengths of both Ridge and Lasso. It’s useful when you have groups of related features and want to either keep or remove them together. If you’ve tried Ridge and Lasso separately and weren’t happy with the results, Elastic Net might give you better predictions.

A good strategy is to start with Ridge if you want to keep all your features. You can move on to Lasso if you want to identify the important ones. If neither gives you good results, then move on to Elastic Net.
