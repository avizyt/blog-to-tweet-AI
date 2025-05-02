# Blog to Tweet AI

**Blog to Tweet AI** is a Python-based tool designed to transform blog articles into concise tweets using advanced language models. This application streamlines the process of summarizing long-form content for social media platforms, particularly Twitter.

## Features

- **Automated Summarization**: Converts blog articles into tweet-sized summaries.
- **Language Model Integration**: Utilizes large language models to ensure coherent and contextually relevant tweets.
- **Modular Architecture**: Structured with separate modules for models, services, and main execution, promoting maintainability and scalability.

## Getting Started

### Prerequisites

- Python 3.8 or higher
- pip package manager
- OpenAI API key (for language model access)

### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/avizyt/blog-to-tweet-AI.git
   cd blog-to-tweet-AI
   ```

2. **Set Up a Virtual Environment (Optional but Recommended)**

   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install Dependencies**

   *(Note: A `requirements.txt` file is not present. Please ensure necessary packages are installed as per your environment.)*

   ```bash
   pip install -r requirements.txt
   ```

   *If `requirements.txt` is unavailable, manually install required packages.*

4. **Set Up Environment Variables**

   Create a `.env` file in the root directory and add your OpenAI API key:

   ```env
   OPENAI_API_KEY=your_openai_api_key
   ```

   Replace `your_openai_api_key` with your actual OpenAI API key.

## Usage

1. **Prepare Input Data**

   Place your blog article content in a file named `article.md` in the root directory.

2. **Execute the Main Script**

   ```bash
   python main.py
   ```

   The script will process the input article and generate tweet-sized summaries, which will be saved in the `twites.txt` file.

## Project Structure

```
blog-to-tweet-AI/
├── __pycache__/           # Compiled Python files
├── .env                   # Environment variables file
├── __init__.py            # Package initializer
├── app.py                 # Application entry point
├── article.md             # Input blog article
├── main.py                # Main script to run the summarization
├── models.py              # Defines data models and structures
├── services.py            # Contains core logic for summarization
├── twites.txt             # Output file containing generated tweets
```

## Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to fork the repository and submit a pull request.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

MIT