1. required->Python: Version 3.10 or higher.
2. ADT Core Library: The system relies on a local, editable installation of adt-core. If you haven't already, install it by running:
        pip install -e C:\KAG\adt-main\adt-core
3. GCP Credentials: The application uses Google GenAI for its language models. Make sure you have Application Default Credentials (ADC) configured for your Google Cloud project.

4. cd C:\KAG\UnifiedRAG
5. copy sample.env .env
6. pip install -r requirements.txt
7. python app.py
8. http://localhost:8002/docs

9. You will see the UnifiedRAG user interface.

Ingest a Document:

Option A (File Upload): Drag and drop a PDF, DOCX, or TXT file onto the "Upload Document" area.
Option B (Paste Text): Copy a block of text and paste it into the "Paste Raw Text" area, then click the Ingest Text button.
Wait for the process to complete. You'll see a success message confirming that the text was ingested and the knowledge graph was denoised. The "Nodes" and "Edges" stats at the top of the page will update.
Query Your Knowledge:

Once your data is ingested, type a question into the "Query the Knowledge Graph" input box.
Click the Ask button.
The AI-generated answer, based on the documents you provided, will appear in the response box below.
You can repeat this process to add more documents and ask more questions. To stop the server, go back to the terminal where it is running and press
