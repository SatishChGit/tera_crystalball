# Teradata Crystal Ball
This project aims to create SQL queries from natural language. 
This sample proof of concept (POC) is centered around tables that exist in the database of the logged-in user within the provided instance. 
It employs the OpenAI gpt-3.5-turbo language model to generate SQL queries based on human input. 
The process involves using the "show table" statement to retrieve the table structure, which is then utilized to construct prompts for the language model. 
The model generates SQL query statements, which are subsequently submitted to Teradata for execution. The results are then displayed as output.

Here are the steps for executing the project:

   1. Clone the project using the command "git clone".
   2. Open the project in PyCharm.
   3. Set up the Run Configurations for "main.py" by adding the following environment variables or define .env at project level  to specify the Teradata instance details and OpenAI API key.
      1. TERADATA_HOST=whomooz;
      2. TERADATA_USER=guest;
      3. TERADATA_PASSWORD=please;
      5. USER_QUERY=query.
      6. AZURE_OPENAI_ENDPOINT=azureendpointurl
      7. AZURE_OPENAI_API_KEY=azurere openai key
      8. AZURE_OPENAI_MODEL=modelname to use
