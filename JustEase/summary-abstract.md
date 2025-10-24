# Summary/Abstract

We are developing a comprehensive **Retrieval-Augmented Generation (RAG) pipeline** for the Department of Justice (DoJ) website to improve citizen access to legal information. Our solution is built on a **multi-representation indexing** approach, where documents are cleaned, summarized, and vectorized for efficient retrieval. By utilizing **sBERT sentence-transformer embeddings**, we ensure that user queries retrieve the most relevant documents based on semantic similarity.

Upon receiving a query, the system goes through **query translation**, using techniques like **multi-query**, **step-back**, and **RAG-fusion** to optimize search results. The query is then routed to the correct database using **logical** or **semantic routing**. The final document retrieval process ensures that the most relevant content is selected and passed to a fine-tuned **LLM** such as **Llama-8B-8191,** **GPT-4o-mini or Command R+** which generates the final response based on the _retrieved context_.

This system is scalable and adaptable, allowing for future enhancements such as **Advanced RAG**, **Adaptive RAG**, and **Corrective RAG**, which will make the system even more efficient and responsive. Our solution will have an intuitive frontend integrated into the DoJ’s website, with plans for broader use across other government departments.

In essence, this solution will empower citizens by providing quick, accurate, and contextually relevant responses to their legal queries, improving their interaction with the judicial system.
