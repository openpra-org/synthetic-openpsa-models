# Synthetic Open-PSA Models
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.13996371.svg)](https://doi.org/10.5281/zenodo.13996371)
<!-- TOC -->
* [Synthetic Open-PSA Models](#synthetic-open-psa-models)
  * [1. OpenPSA Model Exchange Format](#1-openpsa-model-exchange-format)
  * [2. Generation of Models](#2-generation-of-models)
  * [3. Configuration of Models](#3-configuration-of-models)
    * [Configuration 1 `c1-P_0.01-0.05` Arguments and Values](#configuration-1-c1-p_001-005-arguments-and-values)
    * [Configuration 2 `c2-P_0.5-0.9` Arguments and Values](#configuration-2-c2-p_05-09-arguments-and-values)
    * [Configuration 3 `c3-P_0.01-0.9` Arguments and Values](#configuration-3-c3-p_001-09-arguments-and-values)
    * [Configuration 4 `c4-P_0.05-0.9` Arguments and Values](#configuration-4-c4-p_005-09-arguments-and-values)
    * [Configuration 5 `c5-P_0.1-0.9` Arguments and Values](#configuration-5-c5-p_01-09-arguments-and-values)
    * [Configuration 6 `c6-P_0.25-0.9` Arguments and Values](#configuration-6-c6-p_025-09-arguments-and-values)
    * [Configuration 7 `c7-P_0.35-0.9` Arguments and Values](#configuration-7-c7-p_035-09-arguments-and-values)
  * [4. Usage](#4-usage)
  * [5. Additional References Related to Synthetic Models](#5-additional-references-related-to-synthetic-models)
<!-- TOC -->

This repository includes synthetic models in OpenPSA XML format. The goals of including these models are to:

- Serve as test cases for various PRA tools, including [Open-PRA](https://github.com/openpra-org/openpra-monorepo).
- Familiarize users with different modeling approaches and formats.
- Provide a reference for PRA model exchange.
- And more.

The repository also maintains a `schema` for the models and provides four output files for each configuration to give users valuable insights.

## 1. OpenPSA Model Exchange Format
The [OpenPSA Model Exchange Format (MEF)](https://open-psa.github.io/mef/index.html) 
represents about a decade of effort to develop a format independent of any specific 
quantification engine. The goal was to create a standard that researchers, corporations, and regulators could use collaboratively in an open environment.

## 2. Generation of Models
Models are generated leveraging [fault tree generator](https://github.com/rakhimov/scram/tree/develop/scripts)
developed under [SCRAM](https://github.com/rakhimov/scram)


## 3. Configuration of Models
Currently, the generated models are fault tree models. The configurations are listed below. Although 14 options are available for customizing fault trees, the following three arguments are preferred to create fault trees in different formats:

- **The number of basic events**
- **Maximum probability for basic events**
- **Minimum probability for basic events**


### Configuration 1 `c1-P_0.01-0.05` Arguments and Values

| #  | Arguments                                          | Value                     |
|----|----------------------------------------------------|---------------------------|
| 1  | Fault tree name                                    | Autogenerated             |
| 2  | The root gate name                                 | root                      |
| 3  | The seed of the random number generator            | 123                       |
| 4  | **The number of basic events**                     | **100:50:5000**           |
| 5  | The number of house events                         | 0                         |
| 6  | The number of CCF groups                           | 0                         |
| 7  | The average number of gate arguments               | 3.0                       |
| 8  | The weights of gate types [AND, OR, K/N, NOT, XOR] | [1.0, 1.0, 1.0, 0.0, 0.0] |
| 9  | Percentage of common basic events per gate         | 0.3                       |
| 10 | Percentage of common gates per gate                | 0.1                       |
| 11 | The avg. number of parents for common basic events | 2                         |
| 12 | The avg. number of parents for common gates        | 2                         |
| 13 | **Maximum probability for basic events**           | **0.05**                  |
| 14 | **Minimum probability for basic events**           | **0.01**                  |


### Configuration 2 `c2-P_0.5-0.9` Arguments and Values

| #  | Arguments                                          | Value                     |
|----|----------------------------------------------------|---------------------------|
| 1  | Fault tree name                                    | Autogenerated             |
| 2  | The root gate name                                 | root                      |
| 3  | The seed of the random number generator            | 123                       |
| 4  | **The number of basic events**                     | **100:50:5000**           |
| 5  | The number of house events                         | 0                         |
| 6  | The number of CCF groups                           | 0                         |
| 7  | The average number of gate arguments               | 3.0                       |
| 8  | The weights of gate types [AND, OR, K/N, NOT, XOR] | [1.0, 1.0, 1.0, 0.0, 0.0] |
| 9  | Percentage of common basic events per gate         | 0.3                       |
| 10 | Percentage of common gates per gate                | 0.1                       |
| 11 | The avg. number of parents for common basic events | 2                         |
| 12 | The avg. number of parents for common gates        | 2                         |
| 13 | **Maximum probability for basic events**           | **0.9**                   |
| 14 | **Minimum probability for basic events**           | **0.5**                   |


### Configuration 3 `c3-P_0.01-0.9` Arguments and Values

| #  | Arguments                                          | Value                     |
|----|----------------------------------------------------|---------------------------|
| 1  | Fault tree name                                    | Autogenerated             |
| 2  | The root gate name                                 | root                      |
| 3  | The seed of the random number generator            | 123                       |
| 4  | **The number of basic events**                     | **100:50:5000**           |
| 5  | The number of house events                         | 0                         |
| 6  | The number of CCF groups                           | 0                         |
| 7  | The average number of gate arguments               | 3.0                       |
| 8  | The weights of gate types [AND, OR, K/N, NOT, XOR] | [1.0, 1.0, 1.0, 0.0, 0.0] |
| 9  | Percentage of common basic events per gate         | 0.3                       |
| 10 | Percentage of common gates per gate                | 0.1                       |
| 11 | The avg. number of parents for common basic events | 2                         |
| 12 | The avg. number of parents for common gates        | 2                         |
| 13 | **Maximum probability for basic events**           | **0.9**                   |
| 14 | **Minimum probability for basic events**           | **0.01**                  |

### Configuration 4 `c4-P_0.05-0.9` Arguments and Values
| #  | Arguments                                          | Value                     |
|----|----------------------------------------------------|---------------------------|
| 1  | Fault tree name                                    | Autogenerated             |
| 2  | The root gate name                                 | root                      |
| 3  | The seed of the random number generator            | 123                       |
| 4  | *The number of basic events*                       | **100:50:5000**           |
| 5  | The number of house events                         | 0                         |
| 6  | The number of CCF groups                           | 0                         |
| 7  | The average number of gate arguments               | 3.0                       |
| 8  | The weights of gate types [AND, OR, K/N, NOT, XOR] | [1.0, 1.0, 1.0, 0.0, 0.0] |
| 9  | Percentage of common basic events per gate         | 0.3                       |
| 10 | Percentage of common gates per gate                | 0.1                       |
| 11 | The avg. number of parents for common basic events | 2                         |
| 12 | The avg. number of parents for common gates        | 2                         |
| 13 | **Maximum probability for basic events**           | **0.9**                   |
| 14 | **Minimum probability for basic events**           | **0.05**                  |

### Configuration 5 `c5-P_0.1-0.9` Arguments and Values
| #  | Arguments                                          | Value                     |
|----|----------------------------------------------------|---------------------------|
| 1  | Fault tree name                                    | Autogenerated             |
| 2  | The root gate name                                 | root                      |
| 3  | The seed of the random number generator            | 123                       |
| 4  | **The number of basic events**                     | **100:50:5000**           |
| 5  | The number of house events                         | 0                         |
| 6  | The number of CCF groups                           | 0                         |
| 7  | The average number of gate arguments               | 3.0                       |
| 8  | The weights of gate types [AND, OR, K/N, NOT, XOR] | [1.0, 1.0, 1.0, 0.0, 0.0] |
| 9  | Percentage of common basic events per gate         | 0.3                       |
| 10 | Percentage of common gates per gate                | 0.1                       |
| 11 | The avg. number of parents for common basic events | 2                         |
| 12 | The avg. number of parents for common gates        | 2                         |
| 13 | **Maximum probability for basic events**           | **0.9**                   |
| 14 | **Minimum probability for basic events**           | **0.1**                   |

### Configuration 6 `c6-P_0.25-0.9` Arguments and Values
| #  | Arguments                                          | Value                     |
|----|----------------------------------------------------|---------------------------|
| 1  | Fault tree name                                    | Autogenerated             |
| 2  | The root gate name                                 | root                      |
| 3  | The seed of the random number generator            | 123                       |
| 4  | **The number of basic events**                     | **100:50:5000**           |
| 5  | The number of house events                         | 0                         |
| 6  | The number of CCF groups                           | 0                         |
| 7  | The average number of gate arguments               | 3.0                       |
| 8  | The weights of gate types [AND, OR, K/N, NOT, XOR] | [1.0, 1.0, 1.0, 0.0, 0.0] |
| 9  | Percentage of common basic events per gate         | 0.3                       |
| 10 | Percentage of common gates per gate                | 0.1                       |
| 11 | The avg. number of parents for common basic events | 2                         |
| 12 | The avg. number of parents for common gates        | 2                         |
| 13 | **Maximum probability for basic events**           | **0.9**                   |
| 14 | **Minimum probability for basic events**           | **0.25**                  |

### Configuration 7 `c7-P_0.35-0.9` Arguments and Values
| #  | Arguments                                          | Value                     |
|----|----------------------------------------------------|---------------------------|
| 1  | Fault tree name                                    | Autogenerated             |
| 2  | The root gate name                                 | root                      |
| 3  | The seed of the random number generator            | 123                       |
| 4  | **The number of basic events**                     | **100:50:5000**           |
| 5  | The number of house events                         | 0                         |
| 6  | The number of CCF groups                           | 0                         |
| 7  | The average number of gate arguments               | 3.0                       |
| 8  | The weights of gate types [AND, OR, K/N, NOT, XOR] | [1.0, 1.0, 1.0, 0.0, 0.0] |
| 9  | Percentage of common basic events per gate         | 0.3                       |
| 10 | Percentage of common gates per gate                | 0.1                       |
| 11 | The avg. number of parents for common basic events | 2                         |
| 12 | The avg. number of parents for common gates        | 2                         |
| 13 | **Maximum probability for basic events**           | **0.9**                   |
| 14 | **Minimum probability for basic events**           | **0.35**                  |

## 4. Usage
These models can be used to test quantification engines. Additionally, they enable the creation of a verification platform between quantification engines, allowing developers or practitioners to cross-check their results. Moreover, these models serve as a foundation for benchmarking efforts for any quantification tool.


## 5. Additional References Related to Synthetic Models

- E. M. Aras, “Enhancement Methodology for Probabilistic Risk Assessment Tools through Diagnostics, Optimization, and Parallel Computing,” Doctor of Philosophy, North Carolina State University, Raleigh, North Carolina, 2024. [Online]. Available: https://repository.lib.ncsu.edu/items/bb05f7f5-1cff-4beb-9312-331bc94b0b95
- E. M. Aras, A. S. Farag, A. Earthperson, and M. A. Diaconeasa, “Methodology and Demonstration for Performance Analysis of a Probabilistic Risk Assessment Quantification Engine: SCRAM,” in 18th International Probabilistic Safety Assessment and Analysis (PSA 2023), Knoxville, TN: American Nuclear Society, 2023, pp. 452–459.
- E. M. Aras, A. S. Farag, A. Earthperson, and M. A. Diaconeasa, “Method of Developing a SCRAM Parallel Engine for Efficient Quantification of Probabilistic Risk Assessment Models,” in 18th International Probabilistic Safety Assessment and Analysis (PSA 2023), Knoxville, TN: American Nuclear Society, 2023, pp. 134–140.
- E. M. Aras, A. S. Farag, A. Earthperson, and M. A. Diaconeasa, “Benchmark Study of XFTA and SCRAM Fault Tree Solvers Using Synthetically Generated Fault Trees Models,” in Volume 9: Mechanics of Solids, Structures, and Fluids; Micro- and Nano-Systems Engineering and Packaging; Safety Engineering, Risk, and Reliability Analysis; Research Posters, Columbus, Ohio, USA: American Society of Mechanical Engineers, Oct. 2022, p. V009T14A016. doi: 10.1115/IMECE2022-95783.
- A. Farag, S. Wood, A. Earthperson, E. Aras, J. Boyce, and M. Diaconeasa, “Evaluating PRA Tools for Accurate and Efficient Quantifications: A Follow-Up Benchmarking Study Including FTREX,” in Advanced Reactor Safety (ARS), Las Vegas, NV: American Nuclear Society, 2024, pp. 573–582. doi: 10.13182/T130-43377.
- A. S. Farag, E. M. Aras, A. Earthperson, S. T. Wood, and J. Boyce, “Preliminary Benchmarking of SAPHSOLVE, XFTA, and SCRAM using Synthetically Generated Fault Trees with Common Cause Failures,” in 18th International Probabilistic Safety Assessment and Analysis (PSA 2023), Knoxville, TN: American Nuclear Society, 2023, pp. 40–49.




