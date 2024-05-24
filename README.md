# Bias In, Bias Out: Propagation of Representational Intersectional Social Group Bias to Zero-Shot Tasks in Vision-Language Models

This repository contains the code and supporting data for the paper "Bias In, Bias Out: Propagation of Representational Intersectional Social Group Bias to Zero-Shot Tasks in Vision-Language Models". Code to be updated shortly.

## Abstract

In this study, we investigate how social group biases inherent in the representational spaces of vision-language models (VLMs) propagate to downstream zero-shot tasks, focusing on six intersectional race and gender groups: “Asian Men”, “Asian Women”, “Black Men”, “Black Women”, “White Men”, and “White Women”. We use the Chicago Face Database (CFD) for social group signals and the Open Affective Standardized Image Set (OASIS) for valence signals, analyzing biases in models such as CLIP-B-32, CLIP-L-14, and BLIP2.

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

