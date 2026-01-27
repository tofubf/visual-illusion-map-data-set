# Visual Illusion Map Dataset

## Overview
This repository contains a human-verified dataset of choropleth maps constructed to evaluate the color perception capabilities of Large Vision-Language Models (LVLMs). The study investigates whether artificial visual systems exhibit human-like perceptual biases (color illusions) when interpreting cartographic information.

The dataset comprises six distinct types of maps, categorized by the optical illusion mechanism (Neighborhood Contrast, Background Attribution, Stripe Frequency) and the data classification method (Classed vs. Sequential). All data has been manually verified to ensure the validity of the visual illusions while maintaining cartographic integrity.

## Dataset Structure
The dataset is organized into six folders. Each category corresponds to a specific experimental condition designed to test resistance to contextual interference.

### 1. Neighborhood Contrast Illusion (NCI)
Based on the simultaneous contrast effect, where the perception of a target color is shifted by the brightness or hue of its immediate neighbors (induction field).
* **Folders:**
  * `邻域对比分类分级地图` (Neighborhood Contrast - Classed)
  * `邻域对比连续分级地图` (Neighborhood Contrast - Sequential)

### 2. Background Attribution Illusion (BAI)
Investigates assimilation effects (e.g., Bezold-Abney illusion). This tests how overlaying patterns or specific background contexts influence the perceived hue or value of the base regions.
* **Folders:**
  * `背景归因分类分级地图` (Background Attribution - Classed)
  * `背景归因连续分级地图` (Background Attribution - Sequential)

### 3. Stripe Frequency Brightness Illusion (SFBI)
Examines the impact of spatial frequency and brightness of texture patterns on color perception. High or low-frequency stripes are used to induce assimilation or contrast effects respectively.
* **Folders:**
  * `条带频率分类分级地图` (Stripe Frequency - Classed)
  * `条带频率连续分级地图` (Stripe Frequency - Sequential)

## Evaluation Tasks
The dataset is designed to support two primary evaluation tasks for MLLMs:

1. **Classification Task (Classed Maps):**
   The model must identify the correct hue category of a target region. This tests the model's ability to maintain color constancy despite illusory interference.

2. **Quantitative Task (Sequential Maps):**
   The model must estimate the brightness or saturation value (order) of a target region. This evaluates the precision of the model's value judgment under varying contextual backgrounds.

## Usage Notes
* **No Legend:** All map images in this repository are provided without legends (`no_legend`). This setting forces the model to rely solely on visual perception of the map regions, serving as a benchmark for visual grounding capabilities.
* **Ground Truth:** The dataset design includes controlled variable settings to facilitate comparison between illusion-induced errors and ground truth values.

## License
This dataset is released for academic and research purposes.