---
layout: default
title: Editing with Diffusion Transformers
---

# Editing with Diffusion Transformers
### *Understanding Layer Semantics, Attention Pathways, and Spatial Control*  
**Aadya Arora – Research Intern, IISc Bangalore**  
Mentor: Prof. Venkatesh Babu

---

## 🔍 Overview

Diffusion Transformers (DiTs) represent the next generation of text-to-image diffusion models, replacing the U-Net backbone with a fully transformer-based architecture. While they achieve exceptional synthesis quality, the internal functioning of DiTs — *which layers control structure, which layers control semantics, and which layers control local texture* — remains largely unexplored.

This project presents a **comprehensive analysis** of DiTs through:

- 🧩 **Layer-wise ablations** to identify structural, semantic, and detail-oriented layers  
- 🌐 **Unified Attention Mask** for region-specific editing  
- 🖼 **Regional prompting** with fine-grained spatial control  
- 🎭 **DreamBooth + LoRA** personalization experiments across depth  
- 📊 **Replicating Stable Flow** and extending it for DiT architectures  

The findings provide insight into how transformer-based diffusion models encode compositionality, spatial reasoning, and visual identity.

---

## 🧪 Key Experiment Categories

Each component of the project is described in detail on dedicated pages:

- [Layer-wise Ablations](ablations.md)  
- [Regional Prompting](regional_prompting.md)  
- [Unified Attention Mask](regional_prompting.md#unified-attention-mask)  
- [DreamBooth + LoRA](lora.md)  
- [Dataset & Training Setup](dataset.md)  

---

## 🌟 Representative Results

Below are representative results that capture the essence of the project.

### 1. Layer Ablation Sensitivity  
Layers early in the model influence **global structure**,  
middle layers encode **semantics & pose**,  
late layers refine **texture and color**.

**Image required:**  
➡ Extract from PDF page 1 → name it:  
`assets/ablations/cat_grid.jpg`

```markdown
<img src="assets/ablations/cat_grid.jpg" width="700">
*Figure: Ablating individual layers drastically changes the resulting cat images — showing how depth corresponds to structure, semantics, or texture.*
