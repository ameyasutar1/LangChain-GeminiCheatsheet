  <h1>🚀 Gemini + LangChain Cheatsheet</h1>
  <p><strong>A hands-on starter guide to integrating Google's Gemini models with LangChain for multimodal AI applications.</strong></p>

  <h2>📌 Overview</h2>
  <p>This project serves as a comprehensive cheatsheet for developers aiming to harness the power of Google's Gemini models within the LangChain framework. It provides practical examples and code snippets to facilitate the development of AI applications that can process and generate text, images, audio, and video.</p>

  <h2>🧰 Features</h2>
  <ul>
    <li><strong>Text Generation:</strong> Implement chat functionalities using Gemini's language models.</li>
    <li><strong>Multimodal Inputs:</strong> Process and interpret images, audio, and video inputs.</li>
    <li><strong>Prompt Templates:</strong> Utilize LangChain's prompt templates for dynamic input handling.</li>
    <li><strong>Embeddings:</strong> Generate and use text embeddings for semantic understanding.</li>
    <li><strong>Tool Integration:</strong> Incorporate external tools and APIs to extend capabilities.</li>
    <li><strong>Token Usage Tracking:</strong> Monitor and manage token consumption for cost-effective development.</li>
  </ul>

  <h2>🛠️ Installation</h2>
  <p><strong>Clone the Repository:</strong></p>
  <pre><code>https://github.com/ameyasutar1/LangChain-GeminiCheatsheet.git
  cd gemini-langchain-cheatsheet</code></pre>

  <p><strong>Create a Virtual Environment:</strong></p>
  <pre><code>python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate</code></pre>

  <p><strong>Install Dependencies:</strong></p>
  <pre><code>pip install langchain-google-genai numpy </code></pre>

  <p><strong>Set Up Environment Variables:</strong></p>
  <ul>
    <li>Obtain your Google API key from <a href="https://makersuite.google.com/" target="_blank">Google AI Studio</a>.</li>
    <li>Create a <code>.env</code> file in the project root:</li>
  </ul>
  <pre><code>GOOGLE_API_KEY=your_api_key_here</code></pre>

  <h2>📂 Project Structure</h2>
  <pre><code>gemini-langchain-cheatsheet/
├── examples/
│   ├── text_generation.py
│   ├── image_processing.py
│   ├── audio_analysis.py
│   └── video_captioning.py
├── embeddings/
│   └── generate_embeddings.py
├── tools/
│   └── integrate_tool.py
├── utils/
│   └── token_tracker.py
├── requirements.txt
└── README.md</code></pre>

  <h2>🚀 Getting Started</h2>
  <p><strong>Text Generation Example:</strong></p>
  <pre><code>from langchain_google_genai import ChatGoogleGenerativeAI

llm = ChatGoogleGenerativeAI(model="gemini-2.0-flash")
response = llm.invoke("Hello, how can I assist you today?")
print(response.content)</code></pre>

  <p><strong>Image Processing Example:</strong></p>
  <pre><code>from langchain_google_genai import ChatGoogleGenerativeAI
from PIL import Image

llm = ChatGoogleGenerativeAI(model="gemini-2.0-flash")
image = Image.open("path_to_image.jpg")
response = llm.invoke(image)
print(response.content)</code></pre>

  <p><em>Note: Replace <code>"path_to_image.jpg"</code> with the actual path to your image file.</em></p>

  <h2>📖 References</h2>
  <ul>
    <li><a href="https://www.philschmid.de/gemini-langchain-cheatsheet" target="_blank">Google Gemini LangChain Cheatsheet by Philschmid</a></li>
    <li><a href="https://python.langchain.com/docs/" target="_blank">LangChain Documentation</a></li>
    <li><a href="https://makersuite.google.com/" target="_blank">Google AI Studio</a></li>
  </ul>

  <h2>🤝 Contributing</h2>
  <p>Contributions are welcome! If you have examples, enhancements, or suggestions, feel free to open an issue or submit a pull request.</p>

</body>
</html>
