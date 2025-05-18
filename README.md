# Healthcare RAG Agent

The Healthcare RAG Agent is an AI-powered chatbot using RAG, LangChain, Neo4j, and OpenAI GPT, built with Real Python's LLM RAG Chatbot Dataset.

P.S. The chatbot-api folder does not contain any api keys :) It was just named like that for convenience, don't worry.

## Why don't you check it out?

Start by cloning this repo and adding a `.env` file with the following environment variables:

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
You can use the latest gpt-4o-mini instead of the gpt-3.5.

Next, navigate to the project root, start Docker, make sure your AuraDB instance is up and running, and then run:
```bash
make build
```
The build will start the servers, however, you can also start the server with the command:

```bash
make start
```
and stop all containers by running:

```bash
make stop
```
You can interact with the chatbot API docs on localhost:8000/docs, and the UI on localhost:8501:

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
