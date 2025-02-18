# Transformer Model for seq2seq

This repository, **transformer-from-scratch**, provides a complete implementation of a Transformer model built from scratch for sequence-to-sequence tasks. It features both an encoder and a decoder with a linear output layer. The model is designed to handle various NLP tasks such as translation, summarization, and other sequence mapping applications.

## Table of Contents

- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Demo Video](#demo-video)
- [References](#references)

## Usage
```bash
1. Clone the repository:
git clone https://github.com/VatsAmanJha/transformer-from-scratch.git
cd transformer-from-scratch
```

## Model Architecture

The transformer architecture consists of the following components:

- **Encoder**: The encoder processes the input sequence and generates a set of feature representations.
- **Decoder**: The decoder takes the encoder's output and produces the output sequence.
- **Linear Layer**: The final linear layer maps the decoder's output to the desired output shape.

### Model Summary
```plane
Layer (type:depth-idx)                             Param #
===========================================================================
Transformer                                        --
├─EncoderSequence: 1-1                             --
│    └─ModuleList: 2-1                             --
│    │    └─Encoder: 3-1                           7,348,736
├─DecoderSequence: 1-2                             --
│    └─ModuleList: 2-2                             --
│    │    └─Decoder: 3-2                           8,137,728
├─Linear: 1-3                                      1,297,890
===========================================================================
Total params: 16,784,354
Trainable params: 16,784,354
Non-trainable params: 0
===========================================================================
```

## Demo Video

Check out the demo video below for a quick overview of how the transformer model works, along with its implementation and results.

[Transformer Demo Video](demo.mp4)



## References

This work is based on several influential resources in the field of transformers and sequence-to-sequence learning. Special thanks to the following:

- **Attention Is All You Need (Vaswani et al., 2017)**  
  [Arxiv Paper](https://arxiv.org/pdf/2204.13154)
  
- **Illustrated Transformer** by Jay Alammar  
  [Blog Post](https://jalammar.github.io/illustrated-transformer/)
  
- **A Complete Guide to Transformers** by Alejandro Ito Aramendia  
  [Medium Post](https://medium.com/@alejandro.itoaramendia/attention-is-all-you-need-a-complete-guide-to-transformers-8670a3f09d02)

- **YouTube Playlist** 
  [Playlist 1](https://www.youtube.com/playlist?list=PLTl9hO2Oobd97qfWC40gOSU8C0iu0m2l4)

- **YouTube Playlist**  
  [Playlist 2](https://www.youtube.com/playlist?list=PLKnIA16_RmvYuZauWaPlRTC54KxSNLtNn)
