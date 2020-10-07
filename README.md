# Example neuronal data from an economic decision-making task

A subset of processed data from one of our recent experiments featured in Nature Neuroscience ([link](https://pubmed.ncbi.nlm.nih.gov/30258238/)). The full dataset (unprocessed) is publicly available [here](https://crcns.org/data-sets/pfc/pfc-7/about-pfc-7). 

#### Data consists of the following files: 
- x.npy
	- [neurons x trials] matrix of the value of the attended cue
	- Cue was drawn from a set of 5 different values, equally spaced

- y.npy 
 	- [neurons x trials x time] matrix of neural activity during the trial
	- Time is sampled every 10 ms
	- Cue onset is at 500 ms (i.e. point 50)

#### Notes
 - Neurons are from different sessions, and so have different X properties. 

- Only one neuron actually has enough trials to fill the matrix. 

- The other neuron's matrices are padded with NaNs at the later rows which will need to be removed/handled appropriately.