# invoice-rag-app

An end-to-end Retrieval-Augmented Generation (RAG) application that ingests invoices, indexes them efficiently, and enables accurate, context-grounded question answering.

### Links:

[What is Retrieval-Augmented Generation (RAG) ?](https://www.geeksforgeeks.org/nlp/what-is-retrieval-augmented-generation-rag/)

[Advanced RAG: Architecture, techniques, applications and use cases and development](https://www.leewayhertz.com/advanced-rag/)

- document has table, how you convert table to sentances and which package will be used
- pdf plumber of camlet
- how to extract table from pdf and convert to sentances
- does the chunking size for splitting worked well to retrive relevant information from table
- in real world project this work but does not give good accuracy, context recall
- try converting table into json and then convet the sentances and see the results
- how to convert table into json
- use camelot to extract table from pdf and convert to json
- then convert json to sentances

### Python packages for pdf loader

- lanchain_community document loader, directory loader class and pypdfloader class
- pdfplumber
  - preserve table, more appropriate for columns alignments
  - used for financial tables
- unstructred
  - auto detect doucment elements
  - handels header, footers, tables
  - langchain communit document laoder unstrcuted class
  - mixex pdf types
  - higher accuracy in RAG
- OCR for scanned invoice
  - pytesseract package from python
  - good for paper invoice
  - old scanned pdf

### Task

- document abstraction
- chunking
- embedding
- Retrival

![RAG Architecture](/doc/img/rag_architecture.jpeg)
