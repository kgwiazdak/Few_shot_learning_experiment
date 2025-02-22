# Few shot learning experiment
Few shot learning detection experiment related to problem 201 from "200 Concrete Problems In Interpretability Spreadsheet"

## Overview
This repository contains code and experiments related to Few-Shot Learning using transformer-based models. The primary focus is on analyzing the causal contributions of attention and MLP layers in model predictions. The notebook leverages transformer_lens to visualize and quantify the importance of different layers in a few-shot learning setting.

## Features
- Causal Analysis: Measures the contribution of different model components (attention heads, MLP layers) to predictions.
- Visualization Tools: Plots attention distributions and causal contributions per layer.
- Intervention Techniques: Implements causal patching to modify activations and analyze their effects.
- Few-Shot Learning Evaluation: Evaluates model behavior in low-data scenarios.

## Insights & Findings

### Key Observations
- **Attention Contributions**: Layers 5 and 8 contribute most significantly.
- **MLP Role**: The MLP layers show moderate impact, suggesting they refine learned representations.
- **Head-Specific Contributions**: Certain heads play a more significant role than others. Head L7H11, L5H5 and L5H8 seems to have the most interesting attention patterns.

### Future Work
- Try different examples and possibly different models as gpt small struggle with math tasks
- Compare different tasks' activation patterns of most important heads
