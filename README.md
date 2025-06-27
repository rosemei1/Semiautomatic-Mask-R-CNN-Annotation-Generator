# Semi-Automatic Annotation for COCO Dataset (Mask R-CNN)

This repository contains a single Jupyter Notebook that helps **semi-automatically annotate a second batch of images** using a pre-trained Mask R-CNN model trained on a smaller, manually annotated first batch.

> _I don't know if it will be useful or not, but I used this code to help me annotate my second batch dataset. I already had a trained model from the first batch, so I thought, why not try to use it to reduce the manual work? Turned out it helped me a lot._

---

## 🔧 How It Works

1. **Train a Model on the First Batch:**
   - Start by manually annotating a small dataset (first batch).
   - Train a Mask R-CNN model (using any implementation that supports COCO format).

2. **Use This Notebook:**
   - This notebook loads your trained model.
   - It then runs predictions on a new set of images (second batch).
   - The predictions are used to generate COCO-style annotations.

3. **Edit/Validate Annotations:**
   - You can manually tweak or validate the auto-generated annotations to improve quality.

---

## 🗂️ Dataset Format

- Both the **first batch** and **second batch** datasets must follow the **COCO format** (JSON annotations).
- This notebook assumes your model supports this format and that your second batch contains only **images** without annotations (initially).

---
