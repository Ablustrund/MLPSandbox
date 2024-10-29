# MLPSandbox
MPLSandbox is an out-of-the-box multi-programming language sandbox designed to provide unified and comprehensive feedback from compiler and analysis tools for LLMs.


<img width="950" alt="image" src="https://github.com/user-attachments/assets/792e9800-ad98-472a-96ff-b78725f94597">

[![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-brightgreen.svg)](./LICENSE)


# Introduction

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
    


# Requirements & Setup

# Usage




## Note
We are working hard to refactor and improve the open-source version of MLPSandbox to closely match the functionality of the version used internally by Meituan LLM Team.

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


