<div align="center">

# Licence Plate Recognition · v2

**Detect · Read · Track · Measure speed** — in images, videos, webcams and live streams.
Latin and Arabic plates, one stable reading per vehicle, everything exported to Excel.

[![Watch the showcase](https://img.shields.io/badge/▶_Watch_the_showcase-38bdf8?style=for-the-badge)](https://nemri-yassine.github.io/licence-plate-recognition-showcase/)
![YOLO11](https://img.shields.io/badge/YOLO11-Ultralytics-0ea5e9?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3.12-3776ab?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-2.14-ee4c2c?style=for-the-badge&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5-5c3ee8?style=for-the-badge&logo=opencv&logoColor=white)

<img src="media/demo.gif" alt="Live analysis: vehicles tracked with their plate and speed" width="100%">

</div>

---

## Four years later

We built the first version of this project in 2022. It worked — sort of: one box per image, noisy text, no tracking.
In 2026 we came back to it with a simple question: *what if an old project is not a finished project?*
Same idea, rebuilt from the ground up with today's models and libraries.

<img src="media/then-vs-now.jpg" alt="Same footage, same frames: 2022 pipeline vs 2026 pipeline" width="100%">

## What it does

| | |
| --- | --- |
| 🎯 **Plate detection** | YOLO11 fine-tuned on licence plates, with tiled zoom for small and distant plates |
| 🔤 **Multilingual reading** | Plate-specialised OCR for Latin plates (60+ countries, with country prediction) and an English/Arabic reader for Arabic-script plates such as Tunisian تونس plates |
| 🧭 **Tracking** | Every vehicle keeps its ID; multi-frame voting turns noisy per-frame guesses into one stable reading |
| ⚡ **Speed estimation** | Road plane calibrated from lane markings (pixels → metres), robust fit over time, occlusion-aware |
| 📊 **Reports** | Excel workbook, CSV, JSON and plate crops, ready for dashboards, analytics or alerts |

<img src="media/multilingual.jpg" alt="Latin and Arabic plates from Tunisia, the UK, Romania and the US" width="100%">

## Speed, on every tracked vehicle

<img src="media/speed-frame.jpg" alt="Vehicles labelled with ID, plate and speed in km/h" width="100%">

## What gets saved

`results.xlsx` contains four sheets: **Vehicles** (plate, country, OCR confidence, average/max speed, time tracked),
**Plates**, **Speed log** (position and speed of every vehicle on every frame) and **OCR readings**.

<img src="media/excel-report.jpg" alt="Vehicles sheet of the Excel report" width="100%">

## Under the hood

<img src="media/under-the-hood.jpg" alt="Technology stack" width="100%">

## 🔒 Source code

This repository is a **public showcase only**. The source code, models and configuration live in a
**private repository**. For access, a demo or a collaboration, contact the authors.

<div align="center">

*An old project is not a finished project. Update it. Evolve it. Grow with it.*

</div>

---

<sub>© 2026 Yassine Nemri and Iheb Lamouchi. All rights reserved. The images and video in this repository may not be
reused without permission.</sub>
