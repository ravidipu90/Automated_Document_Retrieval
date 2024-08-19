# Automated Document Retrieval and Slack Integration using GPT-4

This project demonstrates the integration of GPT-4 with document retrieval and Slack communication. The system processes PDF documents, retrieves relevant information, answers user queries, and automatically sends the responses to a specified Slack channel.

 Features

- PDF Document Retrieval : Processes PDF documents to extract and search for relevant information.
- GPT-4 Integration : Uses GPT-4 to generate accurate responses based on the retrieved information.
- Slack Communication : Automatically sends the generated answers to a Slack channel, facilitating real-time team collaboration.
- Customizable Prompts : Uses predefined templates for rephrasing and answering questions to enhance the accuracy of responses.

Technologies Used

- GPT-4 : For generating natural language responses.
- LangChain : Manages the language model chain for processing input questions and retrieving documents.
- FAISS: A library for efficient similarity search and clustering of dense vectors, used for document retrieval.
- Slack SDK : For sending messages to Slack channels.
- PyPDF : For processing PDF documents and extracting text.
- dotenv : For managing environment variables, such as API keys.

Installation

1. Clone the repository :
   ```bash
   git clone https://github.com/yourusername/automated-document-retrieval-slack.git
   cd automated-document-retrieval-slack

2. Install dependencies:
 pip install -r requirements.txt

3. Set up environment variables:

Create a .env file in the root directory of the project.
Add your OpenAI API key and Slack API token to the .env file:
OPENAI_API_KEY=your-openai-api-key
SLACK_API_TOKEN=your-slack-api-token

Usage
1. Initialize the environment:

Ensure your environment variables are loaded by running:
source .env
2. Run the main script:

The script processes PDF documents, retrieves information, generates responses using GPT-4, and posts the responses to Slack.
python main.py

3.Customize the prompts:

You can modify the standalone_template and answer_template in the code to fit your specific needs.

Example Workflow
Input Question: "What is the name of the company?"
Output in Slack: The system retrieves the relevant information from the PDF document and posts the answer directly to the designated Slack channel.
