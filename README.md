# Developement solution to the second project
Important note: we did not have time to finish, so we just have have a jupyter notebook with the developement of our idea.

### Solution: Evolution Strategies with Neural networks
The idea is based on two methods, like our solution 1: deep neural nets and [evolution strategies](https://blog.openai.com/evolution-strategies/).  
Here, the neural net output a list of numbers corresponding to all numbers that can be tuned to modify the circuit.  
  
To train the network, evolution strategies are used. In a few words, noise is added to the parameters of the neural network. Then, the net produces a given list of numbers to solve the given problem, which are scored according to the library provided for the BDAthlon. This score is then given back to the network to modifiy its parameters such that the score is increased.  
  
The Python library [Keras](https://keras.io/) is used to create the neural net and [evostra](https://github.com/alirezamika/evostra) for the evolution strategies.  

### Run the notebook
You can either look at our notebook on github, which might be easier given we just have a development solution. Alternatively, if you installed the conda virual env for our first solution, you can reuse it and open the notebook with:

```
jupyter notebook
```

As a reminder, the conda env can bet set this way:  
### Prerequisites

The cleaner way to install the prerequisites is to create a conda virtual environment. 

Firt, you can install conda by following the instructions here: https://docs.anaconda.com/anaconda/install/  

Or update it if you already have it installed:

```
conda update conda
```
And then create a virtual env from the yml file:

```
conda env create -f environment.yml

```

You can now activate your virtual env:

```
source activate bda
```
