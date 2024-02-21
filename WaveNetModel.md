# WaveNet Style Model

- Series of convolutional layers
- Raw input waveform given as input to the first convolutional layer
- We are combining the outputs of each conv layer using a `LINEAR MIXER`
- The output of each conv layer acts as the input for the prev conv layer

## The convolutional layer

- Input signal is processed by the dilated causal FIR filter: $ H_k(z^{d_k}) $
  - k: later index
  - $ d_k $: dilation factor (integer)
-

## Terminology

- Kernel: In a CNN is a small matrix of weights that slides over the input data (such as an image), performs element-wise multiplication with the part of the input it is currently on
- Kronecker delta function : ${\displaystyle \delta _{ij}={\begin{cases}0&{\text{if }}i\neq j,\\1&{\text{if }}i=j.\end{cases}}}$
