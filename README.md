# What is the pellet price ?

The price of wood pellets can be quite fluctuating. It is really time consuming to monitor the pellet price to know when it is the most interesting to buy it.

Ideally, we would keep monitoring several sellers of products and then decide when it is the right time to buy and where to buy. Unfortunately, this is time consuming. We want to automate this web scrapping. 

Unfortunately again, the websites of the sellers are not at all standard. Getting information out of these website smay require dedicated handcrafted rules. Fortunately, with the recent advent of Large Language Models (LLM) and Retrieval Augmentation Generation (RAG), it is now possible to deal with a large variety of website structure and ask the LLMs the answer to questions such as : "Given, this webpage, what is the price of the pellets ? How many pellets can you buy for this price ?" and so on.

Morevoer, if you were interested in the fluctuation of the pellet price, you could parse the website snapshots from the [wayback machine](https://web.archive.org/). 

## Design notes

we may be using :

- unstructured for partitionning the page content
- coupled with Llama index , maybe, for RAGs ? Using a [local install with gpt4all ? ](https://colab.research.google.com/drive/16QMQePkONNlDpgiltOi7oRQgmB8dU5fl?usp=sharing) or maybe [langchain with gpt4all ?](https://python.langchain.com/docs/integrations/llms/gpt4all.html)
