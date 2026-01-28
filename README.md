# Visual Illusion Map Dataset

## Overview
This repository contains a human-verified dataset of choropleth maps designed to evaluate the color perception capabilities of Large Vision-Language Models (LVLMs). [cite_start]The study investigates whether artificial visual systems exhibit human-like perceptual biases when interpreting cartographic information[cite: 1, 6, 8]. [cite_start]The dataset focuses on how contextual factors such as surrounding colors and spatial patterns influence color judgment in map reading tasks[cite: 14, 17]. [cite_start]All data has been manually verified to ensure the validity of visual illusions while maintaining cartographic integrity[cite: 28, 141].

## Data Description
The dataset is organized into six folders representing three specific optical illusion mechanisms applied to two distinct map types (Classed and Sequential).

## File Naming Convention
The filenames in this dataset follow a structured format containing key metadata about the map generation parameters.

**Example:** `Aigle_h300_b0.49_A4_B7.png`

* **`Aigle`**: 
  Represents the specific geographic administrative area depicted in the map (e.g., Aigle, Ain, Ardennes).

* **`h300`**: 
  Indicates the base hue angle of the target color in the HSB color space

* **`b0.49` / `s0.47`**: 
  * `b`: Represents the brightness value (used in illusions like Neighborhood Contrast).
  * `s`: Represents the saturation value (used in illusions like Stripe Frequency).
  * *Note: Some filenames may include `rep` (e.g., `rep2`), indicating the repetition frequency of the pattern.*

* **`A4`**:
  The unique index of the primary target region to be evaluated.

* **`B7`**: 
  The unique index of the comparison region or background context.

## License
This dataset is released for academic and research purposes.




