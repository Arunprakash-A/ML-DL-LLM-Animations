# Gradient Based Optimization Algorithms - Visualized
- I have created a set of animations for the DL and LLM lectures taught by Prof. Mitesh Khapra at IIT Madras in the [Deep Learning course](https://cse.iitm.ac.in/~miteshk/CS6910.html).
- I have uploaded the notebook that I used to create these animations (or) you can directly go to colab [here](https://colab.research.google.com/drive/1LEpnHVFpHzuNIFDWS6GCFw4DIKqe2aBu?usp=sharing) 
- That notebook has an implementation for the gradient descent algorithm. You need to modify the update rule for each optimization algorithm. 
- The objective is to get an intuitive idea of the differences in the optimization algorithms with contrived examples.
- You can find all the animations used in the lecture in .mp4 format in the Animations directory
- Here are a few samples

## Gradient Descent
![Alternate image text](animations/GD_2D.gif)

## Momentum Gradient Descent
![Alternate image text](animations/mgd.gif)

## Nesterov Accelarated Gradient Descent
![Alternate image text](animations/nag.gif)

## AdaGrad
![Alternate image text](animations/adagrad.gif)

## Adam
![Alternate image text](animations/nag.gif)

# Histogram of Activations
- Looking at the distribution of activation values always gives us a lot of insights
- This led to the development of normalization techniques, and block-wise quantization strategies (like in DeepSeek-V3)
- Here is an example of visualizing the histogram of activation values in a simple three-layer neural network.
![Alternate image text](animations/activation_bn.gif)

# Histogram of Gradients (not traditional HoG feature)
- Can we train an LLM model using FP8?
- Look at the range of gradients as the training progresses.
- Likely, the values go outside the dynamic range of FP8.
- Come up with tricks, like block scaling as used in DeepSeek-V3.
- Here is the animation of change in gradient vales of the embedding vector corresponding to the word "the"
- Use backward hooks to capture these values
![Alternate image text](animations/gradient_gpt_2.gif)
