---
layout: default
title: Regional Prompting
---

# 🎨 Regional Prompting in Diffusion Transformers

Regional prompting enables **different text descriptions** to modify **different spatial zones** of the generated image.

---

## 🌲 Two-Tree Example

**Image:** PDF Page 7  
`assets/regional/regional_prompting_1.jpg`

<img src="assets/regional/regional_prompting_1.jpg" width="750">

*Left tree → "lush green tree"*  
*Right tree → "autumn orange tree"*  

Shows precise spatial-text alignment.

---

# 🧠 Unified Attention Mask (UAM)

A key contribution of this project is implementing UAM — combining:

- Cross-attention masks  
- Self-attention masks  
- Regional masks (binary maps)  

This produces controllable spatial editing.

---

## ✨ Unified Mask Visualization

**Image:** PDF Page 12–13  
`assets/masks/unified_mask.png`

<img src="assets/masks/unified_mask.png" width="700">

*Shows token interactions restricted within intended spatial zones.*

---

## 🎨 Additional Regional Results

**Image:** PDF Page 17  
`assets/regional/regional_prompting_2.jpg`

<img src="assets/regional/regional_prompting_2.jpg" width="750">
