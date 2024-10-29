# ✨ MPLSandbox
MPLSandbox is an out-of-the-box multi-programming language sandbox designed to provide unified and comprehensive feedback from compiler and analysis tools for LLMs.


<img width="950" alt="image" src="https://github.com/user-attachments/assets/792e9800-ad98-472a-96ff-b78725f94597">

[![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-brightgreen.svg)](./LICENSE)


# 🔍 Introduction

we propose MPLSandbox, an out-of-the-box sandbox designed to provide unified compiler feedback across multiple programming languages.
Additionally, it integrates traditional code analysis tools, delivering comprehensive code information to LLMs from numerous perspectives.
MPLSandbox simplifies code analysis for researchers, and can be seamlessly integrated into LLM training and application processes to enhance the performance of LLMs in a range of code-related tasks.

MPLSandbox consists of three core modules: 

### Multi-Programming Language Sandbox Environment

This Module can provide unified compiler feedback by compiling and executing the code.
The code and unit test samples are sent to the sub-sandbox of the corresponding programming language for isolated execution to obtain compiler feedback. 
The sandbox ensures the program executes safely without jeopardizing the external environment or interrupting the training process

### Code Analysis Module

This module includes multiple traditional analysis tools to offer a comprehensive analysis report from numerous perspectives.
It provides a comprehensive code analysis from multiple perspectives, such as static analysis (i.e., potential bug detection} and code smell analysis) and dynamic analysis (i.e., fuzz testing and efficiency analysis).
Additionally, this module can also assess other input information besides the code, such as evaluating the coverage of unit tests for the code, aiding researchers in improving the quality of these unit tests.

### Information Integration Module

This module integrates compilation feedback and various analysis results to accomplish a range of complex code-related tasks.
It integrates these results for LLMs to improve the quality of generated code and enhance their performance on a range of code-related tasks.
    

# 🛠️ Requirements & Setup

## Prepare the Docker Images

First, users need to deploy the following Docker image addresses on the host machine, and find the corresponding images on Docker Hub through these links (download them using the `docker pull <image_name>` command):

**Python**: [python:3.9.19-bullseye](https://hub.docker.com/layers/python/3.9.19-bullseye/images/sha256-bb38c82c9e4d6c67117ff8aeb8c9b77a2d2de4738fdfbfc865b51438cb8f41d7?context=explore)

**Java**: [openjdk:11.0.12-jdk-bullseye](https://hub.docker.com/layers/openjdk/11.0.12-jdk-bullseye/images/sha256-bc7e88c3db7a96fdc3b7e287dcb6aa9aa3de0c0b14a8038d5a2c45e2c8880e41?context=explore)

**JavaScript: (https://hub.docker.com/layers/node/22-bullseye/images/sha256-6e2c6f34c1a3c2f5ec5ab0dffb8ef2f8e374a44e62cf70661de35f6ee12b09b4?context=explore)

**C++**: [gcc:11.2.0-bullseye](https://hub.docker.com/layers/gcc/11.2.0-bullseye/images/sha256-0ae9c0984bb0c3d7c505bfa473b1e176c3e3cb2eebf96336d4b0e90862e8bc11?context=explore)

**Go**: [golang:1.17.0-bullseye](https://hub.docker.com/layers/golang/1.17.0-bullseye/images/sha256-dab485fcf1a09b226f57f803eb5eeb3d0f69ab0cb4e798d9f945637dbcbf3883?context=explore)

**Rust**: [rust:latest](https://hub.docker.com/layers/rust/latest/images/sha256-30452e4b244d9284fef6472be2296f0043fc8cc7eb177ec9db49c77be96ed2b9?context=explore)

**TypeScript**: (https://hub.docker.com/layers/node/22-bullseye/images/sha256-6e2c6f34c1a3c2f5ec5ab0dffb8ef2f8e374a44e62cf70661de35f6ee12b09b4?context=explore)  

**Bash**: [bash:latest](https://hub.docker.com/layers/bitnami/bash/latest/images/sha256-18cba5e86f39c57b649276f18e2cbcb9b07a32d15939687c2b5a3ee49b3a8182?context=explore)


## Install MPLSandbox

The user can create and install MPLSandbox using the following command:

```bash
git clone git@github.com:Ablustrund/MPLSandbox.git
cd MPLSandbox
pip install -e .
```

# Usage





## Developing
We are working hard to refactor and improve the open-source version of MPLSandbox to closely match the functionality of the version used internally by Meituan LLM Team.

## Citation

```bibtex
TMP
```

```bibtex
@article{dou2024s,
  title={What's Wrong with Your Code Generated by Large Language Models? An Extensive Study},
  author={Dou, Shihan and Jia, Haoxiang and Wu, Shenxi and Zheng, Huiyuan and Zhou, Weikang and Wu, Muling and Chai, Mingxu and Fan, Jessica and Huang, Caishuang and Tao, Yunbo and others},
  journal={arXiv preprint arXiv:2407.06153},
  year={2024}
}
```


