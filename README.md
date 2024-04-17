# Search-For-Movie-Plots
A notebook to develop a prototypical [semantic] search tool that facilitates an efficient exploration of this historical movie database, helping users
discover relevant movies and shows based on their queries and enhancing users' understanding and appreciation of 1920s cinema.

This repo include 3 notebooks that explore 3 different models of differing complexity to achieve this goal.
Under the 'notebook folder':
1. semantic search
2. reranker
3. RAG


I am choosing not to upload my Analysis and Recommendation document on this experiemnt publicly in this repo, however evaluation metrics and brief analysis are included throughtout the notebooks.


The requirements and dependencies to run locally can be found in the file 'requirements.txt.

## Setup
### Dataset
Use the following code to load the dataset. NOTE: the datasets library is accessible through Hugging Face datasets.

from datasets import load_dataset  
ds = load_dataset("Coder-Dragon/wikipedia-movies", split='train[:1000]')

The dataset includes movie titles, plots, genres, actors, and some other information regarding movies. For this experiment we will only focus on the first 1,000 movies, which are movies from the 1920s or earlier. We will also only focus on querying and embedding the titles and plots.

### Usage 
All notebooks were orignially created and adapted in Google Colab. 
If you wish to run the notebooks locally, run them in order to follow the process most clearly and install any packages and dependencies to avoid running into errors.
A HuggingFace account may be necessary to import the data in the exact same way as the code snippet shown above.
