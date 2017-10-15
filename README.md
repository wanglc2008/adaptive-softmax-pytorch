# Adaptive Softmax for PyTorch

This is translation from https://github.com/facebookresearch/adaptive-softmax, described in the paper "Efficient softmax approximation for GPUs" (http://arxiv.org/abs/1609.04309).

You can first download and preprocess text8 dataset by:

```
python download_text8.py
```

then train language model with adaptive softmax:

```
python text8.py
```

or you can train with regular softmax:

```
python text8.py --model=linear
```

I got similar perplexity to regular softmax with adaptive softmax. Currently I couldn't got exact number in the paper, though. (147 vs 151)
