# Plant-Diseases-Classifier-using-FPGA-Accelerated-CNN
Plant diseases are a crucial issue that threatens the field of agriculture. To facilitate the
identification process as opposed to traditional methods, this thesis project developed a plant
diseases classifier that implements deep learning on FPGA. Normally, embedded CNN
applications, like classification, are applied using CPUs or GPUs, however, this results in
reduced performance and power efficiency. Hence, and due to advancements in high level
synthesis (HLS) tools and PYNQ development boards, the PYNQ-Z1 was used in our project. A
9-layer CNN was trained on the New Plant Diseases dataset and tested using Theano
Framework, and an accuracy of 95.14% was achieved. The weights were then obtained and the
RTL for the CNN was generated using HLS. Vivado HLX was then used for creating the block
design and its wrapper, synthesis, generating the bitstream, and finally programming the FPGA.
Communication between the Processing System (PS) and Programmable Logic (PL) on the
board was mainly carried out through AXI4 and DMA protocols. This paper presents the overall
design for the software and hardware implementations along with the general flow needed for
using the hardware through inputting a leaf image from a webcam and through the HDMI cable
to the board and finally, receiving a prediction indicating whether the plant is diseased or
healthy.
