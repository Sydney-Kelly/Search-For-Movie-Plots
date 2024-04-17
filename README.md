# Search-For-Movie-Plots
A notebook to develop a prototypical [semantic] search tool that facilitates an efficient exploration of this historical movie database, helping users
discover relevant movies and shows based on their queries and enhancing users' understanding and appreciation of 1920s cinema.

This repo include 3 notebooks that explore 3 different models of differing complexity to achieve this goal.


# Setup
## Dataset
use the following code to load the dataset. NOTE: the datasets library is accessible through Hugging Face datasets.

from datasets import load_dataset  
ds = load_dataset("Coder-Dragon/wikipedia-movies", split='train[:1000]')

The dataset includes movie titles, plots, genres, actors, and some other information regarding movies. For this experiment we will only focus on the first 1,000 movies, which are movies from the 1920s or earlier. We will also only focus on querying and embedding the titles and plots.

Usage
