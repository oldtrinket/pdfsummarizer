<h2>PDF Summarize</h2>

PDF Summarize is a simple Python application that summarizes the contents of a single PDF file using OpenAI's language model API. If you want to summarize multiple PDF files, you will need to run the app for each file separately.The app has a graphical user interface built with PyQt5, which allows the user to select a PDF file, and then displays a summary of the contents in a text edit widget. 

<h2>Requirements</h2>

Python 3.6 or later 

PyQt5

PyPDF2

OpenAI API key


<h2>Installation</h2>

1. Clone the repository to your local machine using the following command:

     `git clone https://github.com/your-username/pdf-summarizer.git`

2. Navigate to the directory where the repository was cloned.

3. Install the required dependencies by running the following command:

     `pip install -r requirements.txt`

<h2>Usage</h2>
1. Open a terminal or command prompt and navigate to the directory where the repository was cloned.

2. Set your OpenAI API key as an environment variable by running the following command:

      `export OPENAI_API_KEY=<YOUR_API_KEY>`

Replace <YOUR_API_KEY> with your actual OpenAI API key.

Alternatively, you can set your API key directly in the pdfsum.py file by replacing     openai.api_key = os.getenv("OPENAI_API_KEY") with openai.api_key = "<YOUR_API_KEY>".

3. Run the application by running the following command:

      `python pdfsum.py`
    
4. Click the "Select PDF File" button and choose a PDF file to summarize.

5. The summary will be generated and displayed in the text box below the button.

<h2>Troubleshooting</h2>

If you encounter errors related to PyPDF2, make sure you have installed the correct version of PyPDF2 by running 

    `pip install pypdf2==1.26.0.`
    

If you receive a "RateLimitError" from the OpenAI API, it means you have exceeded your current quota. Check your plan and billing details, or wait until your quota resets.
