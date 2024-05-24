# Bias In, Bias Out: Propagation of Representational Intersectional Social Group Bias to Zero-Shot Tasks in Vision-Language Models

This repository contains the code and supporting data for the paper "Bias In, Bias Out: Propagation of Representational Intersectional Social Group Bias to Zero-Shot Tasks in Vision-Language Models". Code to be updated shortly.

## Abstract

How do social group biases (e.g., the association of marginalized race and gender groups with negative attributes) propagate from the representational spaces of vision-language models (VLMs) to downstream tasks? Here, we comprehensively study the propagation of bias by focusing on 6 intersectional race and gender groups: ``Asian Men", ``Asian Women", ``Black Men", ``Black Women", ``White Men", and ``White Women". We conduct 8 experiments that share a common framework of assessing the correlation between intrinsic bias (e.g., the relative association of a social group image with negatively-valenced vs. positively-valenced sentences), and extrinsic bias (e.g., the likelihood of retrieving negatively valenced text for a given group image prompt). Specifically, for intrinsic bias computation, we use the single category-embedding association test to quantify the effect size of bias within the representational spaces of VLMs (specifically, the English-only version of CLIP-B-32, CLIP-L-14 and BLIP2). For instance, in one experiment, we examine how VLMs capture the association between group signals (e.g., group terms in text) and valence signals (e.g., images rated on positivity/negativity) to measure the intrinsic bias of group-valence associations across image-text modalities. Next, extrinsic bias is evaluated through two widely applied downstream zero-shot tasks, namely, image-to-text and text-to-image retrieval. For instance, given a valenced image prompt (e.g., a negatively valenced image from the Open Affective Standardized Image Set), what is the probability of retrieving text related to marginalized groups? The 8 experiments vary in their focus on the direction of bias propagation (four each on image-to-text and text-to-image) and the type of content analyzed (four on valence, and four on group signals). Across experiments, results demonstrate substantial correlations, with a Spearman's rho of 0.83 ± 0.10, between intrinsic and extrinsic bias measures. This pattern is consistent across an exhaustive set of 114 analyses, including for both retrieval directions (image-to-text and text-to-image), for all six social groups, and for three distinct VLMs. Notably, we find that models that are larger and better performing suggest more bias propagation, a finding that is particularly salient given the current trend towards developing increasingly complex AI models. The results provide an understanding of how social group biases in the intrinsic representations of VLMs are reproduced through downstream AI tasks. Such insights are critical for understanding bias in VLMs, informing researchers, practitioners, and policymakers about where and how to intervene to most effectively mitigate bias.

## Data

### Chicago Face Database (CFD)
The CFD database can be downloaded only from the official website: [CFD Database](https://www.chicagofaces.org/).

### Open Affective Standardized Image Set (OASIS)
The OASIS dataset can be downloaded from the open access website: [OASIS Dataset](https://osf.io/6pnd7/).

### Text Templates
The text templates will be added to this repository separately.

## Code

The code for our experiments and analysis will be added to this repository shortly. It will include scripts for:
- Data preprocessing, and creation of the scaled CFD dataset.
- Bias measurement using the single category-embedding association test (SC-EAT)
- Intrinsic and extrinsic bias quantification and subsequent correlation analysis.

## Usage

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/your-repo-name.git
    cd your-repo-name
    ```

2. Download the CFD and OASIS datasets from the links provided above and place them in the appropriate directories.

3. Run the preprocessing scripts to prepare the data for analysis.

4. Execute the bias measurement scripts to compute intrinsic and extrinsic biases.

5. Perform correlation analysis to study the propagation of biases from VLMs' representational spaces to zero-shot tasks.

## Requirements

- Python 3.x
- PyTorch
- Transformers
- Other dependencies as listed in `requirements.txt`

## Results

Our study demonstrates substantial correlations between intrinsic and extrinsic bias measures across various VLMs and social groups. The results provide insights into how biases inherent in VLMs are reproduced in downstream tasks, emphasizing the need for bias mitigation strategies in the development and deployment of AI models.


## License

This project is licensed under the MIT License - see the LICENSE file for details.

