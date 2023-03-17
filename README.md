# VulHCN
This page includes the code and data used in the paper Focus More on the Small Stuff: Hierarchical Attention-based Capsule Network for Robust Vulnerability Detection.

Instructions for code:

Ubuntu Linux22.04，Python3.10，clang15.0.7，llvm15.0.7，cmake15.0.7

torch1.12.1，graphviz2.38.0，networkx2.8.4，gensim4.3.0，numpy1.23.2

Contributions:

1. We propose a novel greedy vulnerability-sensitive keywords selection approach to pinpoint highly suspicious vulnerable snippets and LLVM intermediate code-based representations to extract multi-dimensional and in-depth program features.
2. We design and implement an automatic detection framework VulHCN, a hierarchical attention-based capsule network for vulnerability detection.
3. We prepare a dataset of 57842 functions, including 21662 vulnerable functions and 36280 non-vulnerable functions. These vulnerabilities are from collected from SARD and NVD.

The design of VulHCN

step1. Parsing program source code into LLVM IR form and eliminating programs that cannot be transformed. 

step2. Identifying greedy vulnerability-sensitive keywords. 

step3. Slcing code lines.
