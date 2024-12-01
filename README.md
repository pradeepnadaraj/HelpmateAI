The project should implement all the three layers effectively. It will be key to try out various strategies and experiments in various layers in order to build an effective search system. Let's explore what you need to do in each of the layers, and the possible experimentations that you can perform based on various choices.

The Embedding Layer: The PDF document needs to be effectively processed, cleaned, and chunked for the embeddings. Here, the choice of the chunking strategy will have a large impact on the final quality of the retrieved results. So, make sure that you try out various stratgies and compare their performances.

Another important aspect in the embedding layer is the choice of the embedding model. You can choose to embed your chunks using the OpenAI embedding model or any model from the SentenceTransformers library on HuggingFace.
 
The Search Layer: Here, you first need to design at least 3 queries against which you will test your system. You need to understand and skim through the document, and accordingly come up with some queries, the answers to which can be found in the policy document.

Next, you need to embed the queries and search your ChromaDB vector database against each of these queries. Implementing a cache mechanism is also mandatory.

Finally, you need to implement the re-ranking block, and for this you can choose from a range of cross-encoding models on HuggingFace.
 
The Generation Layer: In the generation layer, the final prompt that you design is the major component. Make sure that the prompt is exhaustive in its instructions, and the relevant information is correctly passed to the prompt. You may also choose to provide some few-shot examples in an attempt to improve the LLM output.
 

Make sure you try out different strategies and models in each layer, and you might be surprised with the variety of top answers retrieved and generated by your system. 

 

Note: You need to test your system with at least 3 self-designed queries that can help you gauge the quality of outputs delivered by your system. Also, as a check, you need to submit the screenshots of the outputs along with the code and documentation. The details of the screenshots that you need to share are provided below.

Top 3 Results from the Search Layer: You need to share 3 screenshots against 3 self-designed queries that clearly showcase the top 3 results/chunks retrieved from the search layer. Please share 1 screenshot for each query and its output.
Final Generated Answer from the Generation Layer: Here, you are required to share 3 screenshots of the same 3 queries with the final output generated by the LLM in the generation layer. Please share one screenshot for each query and its output.

So, overall, you will need to share 6 screenshots.