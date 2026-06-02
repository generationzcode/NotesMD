>RNNs, very interesting applications

- Able to handle sequences in space and time
- ![[Pasted image 20250320121157.png]]
- I am shamelessly pasting images from the ppt :(
- They have a memory - persistent state - that affects the fortcoming computations
- The RNN takes both the output of the last process and the input of the new process as the input for the network and then produces the new output
- ![[Pasted image 20250320121433.png]]
- one to many is used for image to word mapping
- one to one is for classification
- many to one is sequence of words mapped to sentiment
- many to many (first one) is sequence of words mapped on sequence of words (translation)
- many to many (second) is video frames to classifications
## Unfolding of an RNN to feedforward ANN
- this is done to do backpropagation on it
- ![[Pasted image 20250320121819.png]]
- u is the internal state, x is the input and y is the output
- ![[Pasted image 20250320122023.png]]
- The above has W, which is the weight and the node is the activation and threshold
- It's backpropagated through time
- stacked RNNs have issue with vanishing gradient
- The bidirectional RNNs use nodes that send information both ways, so the neurons are split both ways, the output layer can get information from past AND future states
- Exploding gradient problem - error terms accumulate and cause a massive increase in weight values, this causes the network to be unstable
- LSTM units exist and I don't want to study them
- LSTMs can remember from long ago because they can delete and edit memory
- ![[Pasted image 20250320122633.png]]
- thats sigmoid AND tanh lots of activation...
- It can be seen as a gated cell, where the cell can choose to pass on the signal or not by better gates
- You have 3 gates: input gate, forget gate and output gate