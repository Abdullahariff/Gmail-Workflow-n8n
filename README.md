Gmail-Workflow-n8n
This repository contains a simple n8n workflow that uses an AI agent to send an email via Gmail. This project was completed as a task for a bootcamp to demonstrate skills in integrating AI with no-code/low-code platforms.

🚀 Workflow Overview
This n8n workflow is designed to automate the process of sending emails. It's an excellent example of how to combine a powerful AI model with an email service to create a smart and efficient automation.

The workflow consists of the following key steps:

AI Agent: This node serves as the "brain" of the workflow. It's configured to accept a user prompt (the request to send an email) and intelligently extract key information such as the recipient's email address, the subject line, and the body of the message. It uses a Gemini API model to understand natural language prompts.

Gmail Node: This node is responsible for the actual email sending. It is configured with a secure credential that connects to a user's Gmail account using OAuth 2.0 authentication. It takes the information extracted by the AI agent and uses it to construct and send the email.

✨ Key Features
Natural Language Processing: The AI Agent allows a user to send an email using a simple, human-like prompt (e.g., "send an email to test@example.com with the subject 'Hello' and the message 'Hi there!'").

Secure Authentication: The workflow uses OAuth 2.0, ensuring a secure and private connection to the user's Gmail account without storing sensitive password information.

No-Code Automation: Built entirely within n8n, this workflow demonstrates the power of automation without the need to write complex code.

📦 How to Use This Workflow
To use this workflow, you need to import the Gmail Integration.json file into your own n8n instance.

Create a Gemini API Key:

Go to the Google AI Studio or Google Cloud Console to create a Gemini API key.

Create a Google Cloud Project:

Follow the Google Cloud Console instructions to create a new project and configure the OAuth consent screen.

Import the JSON:

In your n8n instance, go to the Workflows page.

Click on the "Add Workflow" button.

Select "Import from JSON" and upload the Gmail Integration.json file from this repository.

Update Credentials:

Open the imported workflow.

Click on the Gmail node and update the credentials with your new Google Cloud Client ID and Client Secret.

