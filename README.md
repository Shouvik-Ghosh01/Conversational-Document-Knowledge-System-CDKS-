# Conversational Document Knowledge System (CDKS)

CDKS is a web application that revolutionizes information retrieval and exploration from PDF documents. It empowers users to ask questions in natural language and receive insigtful answers derived from the content of uploaded PDFs, fostering a conversational approach to document understanding.

Key Features

Conversational Interface:  CDKS provides a user-friendly chat interface, eliminating the need for crafting complex search queries. Interact with your documents in a natural way, just like having a conversation with a knowledgeable assistant.

Multi-Document Retrieval: Gain insights from a collection of PDFs simultaneously, streamlining information gathering. CDKS eliminates the need to search through each document individually, saving you valuable time and effort.

Contextual Awareness:  CDKS leverages the power of context to provide focused and relevant responses.  The system analyzes the conversation history to understand the user's intent and tailor its answers accordingly. This ensures you receive the most relevant information to your specific needs.

Artificial Intelligence Powered:  At the core of CDKS lies the power of machine learning. The system utilizes pre-trained machine learning models, specifically:

Streamlit: A Python framework for rapidly building custom web applications. Streamlit streamlines the development process, allowing you to focus on the core functionalities of CDKS. (Documentation: https://docs.streamlit.io/)
PyPDF2: A Python library for working with PDF documents. PyPDF2 allows CDKS to extract text content from uploaded PDFs, providing the foundation for information retrieval. (Documentation: https://pypdf2.readthedocs.io/)
Langchain: A Python library for building conversational AI systems. Langchain provides the core components for building the conversational interface and information retrieval pipeline within CDKS. (Documentation: https://python.langchain.com/v0.1/docs/integrations/platforms/huggingface/)
langchain.text_splitter.CharacterTextSplitter: This Langchain component splits the extracted PDF text into manageable chunks, facilitating information retrieval.
langchain_community.embeddings.HuggingFaceInstructEmbeddings: This component utilizes pre-trained language models (specifically, the hkunlp/instructor-xl model) to generate informative embeddings from the text chunks. Embeddings are mathematical representations that capture the semantic meaning of text, crucial for information retrieval.
langchain_community.vectorstores.FAISS: This component utilizes the FAISS library to create a vector store, enabling efficient searching of the generated embeddings. The vector store acts as an index for the extracted knowledge from the PDFs.
langchain.memory.ConversationBufferMemory: This component maintains the conversation history, allowing CDKS to leverage context and provide more relevant responses as the conversation progresses.
HuggingFaceHub: This library provides access to pre-trained large language models (LLMs) which power the core information retrieval and response generation capabilities of CDKS. Specifically, CDKS utilizes the google/flan-t5-base model, fine-tuned for informative retrieval tasks. (Documentation: https://huggingface.co/docs/hub/en/index)
Benefits

Improved Research Efficiency: Quickly find the information you need from multiple PDFs without extensive manual searching. CDKS empowers researchers and academics to focus on analysis and interpretation, not time-consuming document navigation.
Enhanced Document Understanding: Gain deeper comprehension of complex documents through interactive exploration. CDKS facilitates a more natural way to engage with documents, fostering a deeper understanding of the content.
Streamlined Workflows: Simplify information retrieval tasks and save valuable time. CDKS eliminates the need for complex search queries and manual document review, streamlining workflows for professionals across various domains.
Target Audience

Researchers and academics
Legal professionals
Business analysts and intelligence specialists
Technical writers and documentation teams



