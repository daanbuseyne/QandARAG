# QandARAG
Experimenting with QandA RAG systems on different datasets. This code contains a simple RAG system trained on 2 different datasets for 2 different purposes: Wikipedia and joke generation.

NOTES: I used the free version of hf and pinecone, which results in lots of errors regarding 'hourly limit used'. Also had to switch between 2 pinecone indexes. I suggest running this notebook index per index and be very mindful when experimenting with training.


RESULT:
The wikipediaRAG works OK. RAG systems are ideal for these kinds of uses especially the 'give source' function can be handy in a lot of situations. Indicates really clearly where it got the information on wikipedia. Very nice that I am able to run stuff like this locally on my macbook M1. Can be interesting in applications around personal data.

The joke RAG does not work good at all. The jokes of the RAG trained model are not better then the pure llm. However the phi3 model is probably not powerfull enough to really generate intelligent jokes AND using RAG does not really make much sense to train a joke generator. I dont think the jokes get more intelligent after the RAG.  However It was fun to train the RAG on a different kind of dataset (short sentences, text split not necessairy). RAG system similar to joke one could be helpfull for quotes regarding subjects if includes with 'get source' function.
