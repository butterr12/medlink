# Healthcare RAG Agent

I decided to build this chatbot with the help of Real Python's LLM RAG Chatbot Dataset.

## Why don't you check it out?

Start by cloning this repo and adding a `.env` file with the following environment variables:

```markdown

```bash
OPENAI_API_KEY=<YOUR_OPENAI_API_KEY>

NEO4J_URI=<YOUR_NEO4J_URI>
NEO4J_USERNAME=<YOUR_NEO4J_USERNAME>
NEO4J_PASSWORD=<YOUR_NEO4J_PASSWORD>

HOSPITALS_CSV_PATH=https://raw.githubusercontent.com/hfhoffman1144/langchain_neo4j_rag_app/main/data/hospitals.csv
PAYERS_CSV_PATH=https://raw.githubusercontent.com/hfhoffman1144/langchain_neo4j_rag_app/main/data/payers.csv
PHYSICIANS_CSV_PATH=https://raw.githubusercontent.com/hfhoffman1144/langchain_neo4j_rag_app/main/data/physicians.csv
PATIENTS_CSV_PATH=https://raw.githubusercontent.com/hfhoffman1144/langchain_neo4j_rag_app/main/data/patients.csv
VISITS_CSV_PATH=https://raw.githubusercontent.com/hfhoffman1144/langchain_neo4j_rag_app/main/data/visits.csv
REVIEWS_CSV_PATH=https://raw.githubusercontent.com/hfhoffman1144/langchain_neo4j_rag_app/main/data/reviews.csv

HOSPITAL_AGENT_MODEL=gpt-3.5-turbo-1106
HOSPITAL_CYPHER_MODEL=gpt-3.5-turbo-1106
HOSPITAL_QA_MODEL=gpt-3.5-turbo-0125

CHATBOT_URL=http://host.docker.internal:8000/hospital-rag-agent
```

### Setting Up

1. **Navigate to the Project Root:**
   
   Make sure you’re in the root directory of the project.

2. **Start Docker:**
   
   Start Docker and ensure your AuraDB instance is up and running.

3. **Build the Project:**

   Run the following command to build the project:

   ```bash
   make build
   ```

   This will start the servers.

4. **Start the Server:**

   Alternatively, if you just want to start the server, use the following command:

   ```bash
   make start
   ```

5. **Stop the Containers:**

   To stop all running containers, use:

   ```bash
   make stop
   ```

### Interact with the Chatbot

You can interact with the chatbot API docs at [localhost:8000/docs](http://localhost:8000/docs), and the UI is available at [localhost:8501](http://localhost:8501).

## Technologies Used

- **LangChain** for creating and managing the knowledge graph.
- **FastAPI** for creating the chatbot API.
- **Streamlit** for the user interface.
- **Neo4j** for storing and querying the knowledge graph.
- **OpenAI GPT** for chatbot interactions.

## Getting Help

If you run into issues, feel free to open an issue here on GitHub, and I’ll do my best to assist you!

## Contributions

Contributions are welcome! If you'd like to improve the project or add new features, feel free to fork the repo, make your changes, and create a pull request.

---

Happy learning and coding! 🚀
```
