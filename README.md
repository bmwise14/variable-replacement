# variable-replacement

The purpose of variable replacement is to enable the discovery of configuration templates across a set of OS device types and customers by de-identifying locally significant variables and keeping globally significant ones.

We do this by training a deep learning model with OS training data using the [BERT](https://github.com/google-research/bert)'s concept of masked language modeling. Our goal is to "mispredict" locally significant variables - like customer PII or other local identifiers - and accuractely predict globally significant non-local words. I am proud to have worked with extremely talented peers and written the model training and evaluation code for this clever use of deep learning.

The source code is property of Cisco and cannot be disclosed. However, the idea itself is public domain and can be read in this defensive publication below:
- [Automating Network Device Configuration Template Discovery](https://www.tdcommons.org/cgi/viewcontent.cgi?article=6437&context=dpubs_series)

