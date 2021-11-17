---
title: Aungemented Reality
summary: Perspective Transform with ArUco marker(OpenCV)
tags:
- Image processing
date: "2021-09-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: 
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
## Introudction
此專案為使用OpenCV實作一AR效果，目標為將任一指定圖片鑲嵌至一原本含有ArUco marker的影片上，上圖為原始影片之截圖。此方法也可以應用至其他日常生活上，例如將3D人物投影至指定位置。其中主要使用了兩個技巧分別為
- HomoGraphy

- Perspective Transform

## Method
- 讀取含有ArUco marker 的原始影片，並針對每一幀處理
  - 抓取每一幀的ArUco marker，並將其(x,y)座標抓取來
- 對每一幀做Perspective Transform
  - find Homography
  - perspective transform
- 輸出成影片檔案

## Result
完成後結果如下所示
{{< video src="my_video.mp4" controls="yes" >}}