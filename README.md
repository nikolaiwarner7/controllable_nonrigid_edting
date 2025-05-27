# AFFORDANCE-DIFFUSION

> A controllable, identity-preserving diffusion model for non-rigid human edits in the wild.

## 📖 Project Description

We address the challenging task of inserting and re-posing people in arbitrary scenes—guided only by a masked target image, a reference person crop, and a text description of the desired pose. Our model:

- **Maintains Identity:** preserves the subject’s appearance via cross-attention on the reference image.  
- **Enables Non-Rigid, Text-Guided Edits:** you can say “He lunges his right leg forward” or “She raises her arms above her head,” and the person’s pose changes accordingly.  
- **Works In-the-Wild:** robust to complex backgrounds and motion blur, validated by a user study that shows a 10% boost in pose adherence (PCKt@0.5) over prior inpainting methods—with no loss in visual fidelity.

We also introduce a new dataset of video-derived frame pairs with scene-difference captions, generated via GPT-4V and filtered by pose estimators to reduce hallucinations.

> **Note:** Code, data, and our automated captioning pipeline will be released here shortly.

## 🚀 Getting Started

1. **Clone:**  
   ```bash
   git clone https://github.com/YOUR_GITHUB_USER/affordance-diffusion.git
   cd affordance-diffusion

This project builds on and extends:

- **Affordance Insertion** by Adobe Research  
  https://github.com/adobe-research/affordance-insertion  
- **Hallucinating Scenes** by Timothy Brooks  
  https://github.com/timothybrooks/hallucinating-scenes  