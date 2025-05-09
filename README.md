# AI Web Scraper

A Streamlit-based web scraping tool that extracts and cleans content from websites using Selenium and BeautifulSoup, with advanced parsing capabilities powered by Ollama and LangChain.


## Features
- Scrape website content using a headless browser (Selenium with Scraping Browser).
- Clean and extract DOM content for analysis.
- Display scraped content in an expandable text area.
- Parse content based on user-defined descriptions using the Ollama language model.
- Persistent session state for seamless interaction.
![Screenshot 2025-05-09 130250](https://github.com/user-attachments/assets/e867a52a-9790-4439-a0f9-7e692f051e6e)


## Prerequisites
- Python 3.8+
- Git (for cloning the repository)
- The following Python packages:
  - `streamlit`
  - `selenium`
  - `beautifulsoup4`
  - `python-dotenv`
  - `langchain-ollama`
  - `langchain-core`

## Installation

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/ai-web-scraper.git
cd ai-web-scraper

2. Install Dependencies
Create a virtual environment and install the required packages:

bash


python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
Note: Create a requirements.txt file with the following content if not already present:

text


streamlit
selenium
beautifulsoup4
python-dotenv
langchain-ollama
langchain-core
3. Set Up Environment Variables
Create a .env file in the project root directory and add the following:

text


SBR_WEBDRIVER=your_scraping_browser_webdriver_url
Replace your_scraping_browser_webdriver_url with the URL of your Scraping Browser WebDriver service.
4. Install and Configure Ollama
Download and install Ollama for Windows from https://ollama.com/.
Add the Ollama binary directory (e.g., C:\ollama) to your system PATH.
Pull a model (e.g., llama3.2) to use for parsing:
bash


ollama pull llama3.2
Usage
1. Start the Ollama Server
Open a Command Prompt and run:




ollama serve
Keep this terminal open while using the app.

2. Run the Streamlit App
In a separate Command Prompt, navigate to the project directory and start the app:

bash


streamlit run main.py
Open your browser and go to http://localhost:8501/ai-web-scraper.
3. Interact with the App
Enter Website URL: Input a URL (e.g., https://techwithtim.net) in the "Enter Website URL" field.
Scrape Website: Click "Scrape Website" to extract and display the DOM content in the expandable "View DOM Content" section.
Describe Parsing: In the "Describe what you want to parse" text area, enter a description (e.g., "extract all headings").
Parse Content: Click "Parse Content" to process the content using the Ollama model based on your description. The result will update the DOM content display.
File Structure
text


ai-web-scraper/
│
├── main.py              # Streamlit app logic
├── scrape.py            # Web scraping functions using Selenium and BeautifulSoup
├── parse.py             # Parsing logic using Ollama and LangChain
├── .env                 # Environment variables (e.g., SBR_WEBDRIVER)
├── requirements.txt     # Python dependencies
└── README.md            # This file
Contributing
Fork the repository.
Create a new branch (git checkout -b feature-branch).
Make your changes and commit them (git commit -m "description").
Push to the branch (git push origin feature-branch).
Open a Pull Request.
License
This project is licensed under the MIT License - see the  file for details.

Acknowledgments
Streamlit for the web app framework.
Selenium for browser automation.
BeautifulSoup for HTML parsing.
Ollama and LangChain for AI-powered parsing.
Inspiration from web scraping tutorials and AI integration projects.
text



### Notes
- **Repository URL**: Replace `https://github.com/your-username/ai-web-scraper.git` with your actual GitHub repository URL.
- **LICENSE File**: Create a `LICENSE` file with the MIT License text if you choose to use it, or specify a different license.
- **Customizations**: Adjust the acknowledgments or add sections (e.g., "Known Issues," "Future Work") as needed.
- **Requirements.txt**: Ensure you generate this file by running `pip freeze > requirements.txt` in your virtual environment after installing dependencies.

Save this as `README.md` in your project root directory, and it will render nicely on GitHub. Let me kn
