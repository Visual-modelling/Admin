
# Visual-modelling
Repo to store high-level [issues](https://github.com/Visual-modelling/Visual-modelling/issues)

See the [Project Board](https://github.com/orgs/Visual-modelling/projects).


## Meeting Notes: 5th March 2020

### **Dataset**

- Hudson has implemented a basic 2d bouncing circle.
- Testing if the model is capable of self learning conservation of momentum and law of reflection by varying the following (as initial PoC):
  - Varying circle size
  - Varying initial velocity and position
    - Constrain the initial velocity to be no more than half the distance between the initial position and the boundary

- This will be tested on CNN and Transformer based models to begin with.

### **Transformer Model**

- Look into potential Pixel Embedding Space.
- Will need for each pixel a positional encoding, and a temporal encoding.
- Positional and temporal can be combined into the same 3D encoding for 2D videos and 4D encoding for 3D videos
- Need to read up on how BERT treat embeddings encodings (relative or not)

Long term dependencies will be a problem in the future, but not within the scope of this initial work - as we are only modeling physical laws which do not require long-term observational memory.

### **Action Points**

- Hudson will incorporate the parameter space search (using the variables described above) to generate the dataset
- Dean will look at whats required for the transformer to do the video prediction task for a sequence of 2D images (positional/temporal encodings + pixel embedding space)
- Zheming will look at the latest techniques used in Vision for video prediction and add to literature review.
