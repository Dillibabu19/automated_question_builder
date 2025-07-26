PDF Question Generator
A Retrieval-Augmented Generation (RAG) application that automatically generates educational questions from PDF documents using AI. Upload a PDF and create various types of questions including multiple choice, fill-in-the-blanks, and questions across different taxonomy levels.

Features
PDF Upload & Processing: Upload PDF documents for content extraction

RAG Implementation: Utilizes Retrieval-Augmented Generation for intelligent question creation

Multiple Question Types:

Multiple Choice Questions (MCQ)

Fill-in-the-blank questions

Various other question formats

Taxonomy Levels: Generate questions across different educational taxonomy levels (Bloom's Taxonomy)

AI-Powered: Leverages OpenAI API for intelligent question generation

Modern UI: React-based frontend for seamless user experience

Tech Stack
Backend
Python: Core backend language

OpenAI API: AI-powered question generation

RAG Framework: For document retrieval and generation

Frontend
React: Modern web application framework

JavaScript/TypeScript: Frontend development

Installation
Prerequisites
Python 3.8+

Node.js 14+

OpenAI API key

Backend Setup
Clone the repository:

bash
git clone <repository-url>
cd pdf-question-generator
Create a virtual environment:

bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install Python dependencies:

bash
pip install -r requirements.txt
Set up environment variables:

bash
cp .env.example .env
# Add your OpenAI API key to .env file
OPENAI_API_KEY=your_openai_api_key_here
Frontend Setup
Navigate to the frontend directory:

bash
cd frontend
Install dependencies:

bash
npm install
Usage
Starting the Application
Start the backend server:

bash
python app.py
Start the frontend development server:

bash
cd frontend
npm start
Open your browser and navigate to http://localhost:3000

How to Use
Upload PDF: Click the upload button and select your PDF document

Select Question Type: Choose from MCQ, fill-in-the-blanks, or other available formats

Choose Taxonomy Level: Select the desired educational taxonomy level

Generate Questions: Click generate to create AI-powered questions

Review & Export: Review generated questions and export if needed

API Endpoints
POST /upload
Upload a PDF document for processing

POST /generate-questions
Generate questions based on uploaded PDF

Parameters:

question_type: Type of questions to generate

taxonomy_level: Educational taxonomy level

count: Number of questions to generate

GET /questions/{id}
Retrieve generated questions by ID

Question Types
Multiple Choice Questions (MCQ): Traditional multiple-choice format

Fill-in-the-Blanks: Questions with missing words/phrases

Short Answer: Brief response questions

Essay Questions: Long-form response questions

Taxonomy Levels
Based on Bloom's Taxonomy:

Remember: Recall facts and basic concepts

Understand: Explain ideas or concepts

Apply: Use information in new situations

Analyze: Draw connections among ideas

Evaluate: Justify a decision or course of action

Create: Produce new or original work

Configuration
Environment Variables
text
OPENAI_API_KEY=your_openai_api_key
DATABASE_URL=your_database_url (optional)
DEBUG=True/False
Customization
You can customize question generation by modifying:

Prompt templates in prompts/

Question types in question_types.py

Taxonomy levels in taxonomy.py

Contributing
Fork the repository

Create a feature branch (git checkout -b feature/amazing-feature)

Commit your changes (git commit -m 'Add some amazing feature')

Push to the branch (git push origin feature/amazing-feature)

Open a Pull Request

License
This project is licensed under the MIT License - see the LICENSE file for details.

Support
If you encounter any issues or have questions, please open an issue on GitHub or contact the development team.

Roadmap
 Support for additional file formats (Word, PowerPoint)

 Question difficulty assessment

 Batch question generation

 Question bank management

 Integration with Learning Management Systems (LMS)

 Multi-language support

Note: Make sure to keep your OpenAI API key secure and never commit it to version control.
