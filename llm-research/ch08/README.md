## Model compression

### Model Optimization
Parameters, Model Size, Activations, MAC,FLOP,OPS, Latency, Throughput
#### Conv Nets
Normalization: Batch Norm, Layer Norm, Instance Norm, Weight Norm, Group Norm
Activation Function (non linear ):Sigmoid, ReLU, LeackyReLU, ReLU6, Swish, Hard Swish
Conv Layer: Output Size= ( Input Size−Filter Size+2×Padding) / Stride + 1


### LLM Compression Training and Inference
Deep Compression: Compressing Deep Neural Networks with Pruning, Trained Quantization and Huffman Coding, https://arxiv.org/abs/1510.00149
![image](https://github.com/user-attachments/assets/fb2c2d0a-f0b5-44bd-9008-5616670037f7)

#### Pruning
Pruning Synapses vs Pruning Neurons
Memory is Expensive: 32 bit DRAM Memroy ~640 pJ vs 32 bit int Add ~0.1 pJ
 - Pruning  at different  Granularities
 - Iterative Pruning
 - Magnitude Based Pruning
 - Scaled based Pruning
 - Second Order Based Pruning
 - Percentage Zero Based Pruning
 - Regression base Pruning
 - Parallelization on Sparsity
 - 

AutoML for Pruning: https://github.com/mit-han-lab/amc

   Hardware support for sparsity:
   - EIE: Efficient Inference Engine on Compressed Deep Neural Network, https://arxiv.org/abs/1602.01528
   - SpAtten: Efficient Sparse Attention Architecture with Cascade Token and Head Pruning, https://arxiv.org/abs/2012.09852
   - NetAdapt: Platform-Aware Neural Network Adaptation for Mobile Applications, https://arxiv.org/abs/1804.03230

  System Support for sparsity:
   - Accelerating Sparse Deep Neural Networks, https://arxiv.org/abs/2104.08378


#### Sparsity
#### Quantization
Neural Network Quantization
 - k-means based quantization
 - weight quantization
 - huffman coding
 - Linear Quantization
 - Quantization Granularity (per-tensor, per-channel, per-group quantization)
 - 

#### Neural Architecture Search
#### Knowledge Distillation
Knowledge distillation is a machine learning technique that involves transferring knowledge from a large, complex model (the "teacher" model) to a smaller, more efficient model (the "student" model). The goal is to enable the student model to achieve similar performance to the teacher model while being more compact and faster to run, which is particularly useful for applications with resource constraints, such as mobile devices or embedded systems.

### On-Device Training

### ML Performance Benchmarks
MLPerf https://mlcommons.org/benchmarks/
MLPerf: Closed Devision / Open Devision / Speedup

## Labs References 
https://github.com/yifanlu0227/MIT-6.5940


## References
1. BEVFusion: Multi-Task Multi-Sensor Fusion with Unified Bird’s-Eye View Representation
2. Lite Transformer with long-short range attention
3. Language Models are Few-Shot Learners
4. Chain-of-Thought Prompting Elicits Reasoning in Large Language Models
5. SpAtten: Efficient Sparse Attention Architecture with Cascade Token and Head Pruning
   Code: https://github.com/mit-han-lab/spatten-llm
6. llama.cpp
   Code: https://github.com/ggerganov/llama.cpp
8. tensor library for machine learning
   Code:https://github.com/ggerganov/ggml
9.TinyChatEngine on device LLM/VLM
   Code:https://github.com/mit-han-lab/TinyChatEngine/
10. AWQ: ACTIVATION-AWARE WEIGHT QUANTIZATION FOR ON-DEVICE LLM COMPRESSION AND ACCELERATION
11. Book:Efficient Processing of Deep Neural Networks. https://link.springer.com/book/10.1007/978-3-031-01766-7
12. Recipe: https://karpathy.github.io/2019/04/25/recipe/
13. DNN http://csg.csail.mit.edu/6.5930/readinglist.html
14. Intro Deep Learning MIT http://introtodeeplearning.com/
15. Computer Vision: Algorithms and Applications, 2nd ed

### AI / DL Courses:
Efficient Deep Learning Computing https://hanlab.mit.edu/courses/2023-fall-65940
Alex Smola https://d2l.ai/
Computer Vision https://advances-in-vision.github.io/schedule.html
Noah Snavely's CS5670 - Introduction to Computer Vision class at Cornell Tech (Spring 2023)
Bill Freeman, Antonio Torralba, and Phillip Isola's 6.8300/6.8301: Advances in Computer Vision class at MIT (Spring 2023)
Yasutaka Furukawa's CMPT 412 - Computer Vision class at Simon Fraser University (Spring 2023)
David Fouhey's EECS 442: Computer Vision class at the University of Michigan (Winter 2023)
Alyosha Efros' CS194-26/294-26: Intro to Computer Vision and Computational Photography class at Berkeley (Fall 2022)
James Hays' CS 4476-A / 6476-A Computer Vision class at Georgia Tech (Fall 2022)
James Tompkin's CSCI 1430 Computer Vision class at Brown (Spring 2023)
Ioannis Gkioulekas's 15-463, 15-663, 15-862 Computational Photography class at CMU (Fall 2023)
Matthew O'Toole's 16-385 Computer Vision class at CMU (Fall 2022)
Justin Johnson's EECS 498.008 / 598.008: Deep Learning for Computer Vision class at the University of Michigan (Winter 2022), which is an outstanding introduction to deep learning and visual recognition
Yann LeCun and Alfredo Canziani's DS-GA 1008: Deep Learning class at NYU (Spring 2021)
Luiz Velho's Fundamentals and Trends in Vision and Image Processing class at IMPA (Spring 2021)
UC Berkeley's CS294-158-SP20: Deep Unsupervised Learning class (Spring 2020)
Scott Wehrwein's CSCI 497P/597P - Introduction to Computer Vision class at Western Washington University (Spring 2020)
Andrew Owens' EECS 504: Foundations of Computer Vision class at the University of Michigan (Winter 2020)

### Image/ Video Processing libraries (cameras, embedded, etc)
https://facebookresearch.github.io/ocean/
https://arxiv.org/abs/2407.13764 4D reconstruction



