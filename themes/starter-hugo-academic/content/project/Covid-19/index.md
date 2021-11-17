---
title: Covid-19 Prediction
summary: An example of using the in-built project page.
tags:
- Deep Learning
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

## Introduction
該專案為預測美國地區Covid-19案件個數。藉由觀察美國某一洲過去三天的變數來預測該洲別第4天的Covid陽性百分比。
其中，變數包括了行為因素、精神健康因素、是否有得到類似Covid疾病以及味覺因素共18項。

## Method

該專案使用DNN Model 其中激勵函數使用 ReLU，並使用Adam調整learning rate的收斂。

## Result
{{< figure src="Covid.png" title="Learning rate curve" >}}
{{< figure src="predict.png" title="predict vs ground true value" >}}

