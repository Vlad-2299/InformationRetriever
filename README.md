# InformationRetriever
Cosmology-Based Question &amp; Answer System


![alt text](https://github.com/Vlad-2299/InformationRetriever/blob/master/model.png?raw=true)


<h2>Elastic Search Local Server</h2>
Ensure to install https://www.elastic.co/pt/elasticsearch/ and run as administrator, before executing the system; <br>
Used version==7.11.2

<h2>PDF_Reader.ipynb</h2>
Reads and processes all the PDF files inside RawPapers. Outputs a TXT file into ProcessedData, with the text content of the PDF file.

<h2>Web_Scraper.ipynb</h2>
Reads and processes all the HTML pages inside RawWebPages. Outputs a TXT file into ProcessedData, with the text content of the web page.

<h2>DataStore.ipynb</h2>
Ensures that a connection with ElasticSearch is established. Reads the saved content in ProcessedData, and for each passage, creates a JSON document which will be used to populate the DocumentStore.

<h2>Retriever_Reader.ipynb</h2>
Deploys three off-the-shelf models: Pegasus (Question reformulator), BM25Retriever (Document retriever), RoBERTa (Document reader)
