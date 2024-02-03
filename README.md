# FYP
## Query Based Video Summarization

### Contextualized Video Summary Controller (query_embeddings.ipynb)
This notebook contains the code for generating embeddings of QV Highlight & TVSUM Queries.

highlight_train_release -> this json file contains queries of QV Highlight Dataset.

tvsum_train -> this json file contains queries of TVSUM Dataset.

The contextualized video summary controller integrates a transformer-encoder and a transformer-decoder which takes a user query as an input. This architecture consists of DistilBERT. The self-attention mechanism helps to capture relationships between tokens in the input sequence. In order to prepare the user query for input into the DistilBERT model, a series of preprocessing steps are applied. This includes text cleaning, where the raw text of the user query is subjected to procedures like lowercasing, removal of stopwords, extra spaces and special characters. These preprocessing steps help to refine the input text, enhancing the model’s ability to generate meaningful embeddings for video summarization. These cleaned and pre processed queries are used by this pretrained model to generate embeddings. These embeddings will further be used by feature fusion models.


### Code for UI is linked with Google Drive so you will need to do the following

1) mount the notebook to your google drive account
2) update the path for the file storage i.e. path to the directory
3) update the path where the file will go to i.e. output directory 

