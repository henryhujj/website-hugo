---
title: Video tracking
summary: An example of using the in-built project page.
tags:
- Image processing
date: "2021-09-10T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: 
  focal_point: Smart

links:
//- icon: 
  icon_pack: 
  name: 
  url: 
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
此專案的目標為追蹤影片中的斑點並製作一Optical Flow(光流)。
## Method
- 讀取影片
- 抓取影片中的斑點位置設為特徵點
- 讀取新的一幀後，和上一幀的特徵點計算他們的差異，並繪圖(Optical Flow)
## Result

{{< video src="my_video.mp4" controls="yes" >}}