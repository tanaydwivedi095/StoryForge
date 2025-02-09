# StoryForge - Intelligent Storytelling Assistant

## Overview
The **StoryForge - Intelligent Storytelling Assistant** is a Jupyter Notebook-based application that generates short children's stories with moral values and creates relevant illustrations for them using AI models. It ensures the stories are engaging, simple, and appropriate for young readers by incorporating different animal characters and curiosity-driven narratives.

## Features
- **Automated Story Generation**: Uses OpenAI's GPT-3.5-turbo-16k to generate short children's stories featuring different animal characters.
- **Illustration Prompt Extraction**: Extracts key illustration prompts from the generated story to guide an AI-based illustration tool.
- **AI-Powered Image Generation**: Uses the Segmind SDXL model to generate relevant story illustrations in a selected artistic style (e.g., "kawaii").
- **Gradio UI**: Provides an interactive interface for viewing the generated stories alongside their respective illustrations.

## Technologies Used
- **Python**: Core programming language for handling story and image generation.
- **Jupyter Notebook**: The environment used for developing and running the project.
- **OpenAI GPT-3.5-turbo-16k**: For generating children's stories based on predefined prompts.
- **Segmind SDXL**: AI-powered illustration model to generate high-quality images.
- **Gradio**: For building an interactive web UI to showcase the generated stories and illustrations.
- **Requests & JSON**: For handling API interactions and data processing.
- **Matplotlib & PIL**: For image display and manipulation.

## Installation
### Prerequisites
Ensure you have Python installed (version 3.8 or later). Install the required dependencies:

```sh
pip install requests gradio matplotlib pillow segmind jupyter
```

### API Keys Setup
You will need API keys for OpenAI and Segmind. Set them up securely using `getpass`:

```python
from getpass import getpass
openaikey = getpass('Enter your OpenAI API Key: ')
segmindkey = getpass('Enter your Segmind API Key: ')
```

## Usage
1. **Run the Jupyter Notebook**:

```sh
jupyter notebook
```

2. **Generate a Story**:
   - The notebook fetches a short children's story from OpenAI based on predefined prompts.
   - The story is structured with a title and narrated using different animal characters.

3. **Extract Illustration Prompts**:
   - The application generates a set of one-line descriptions for illustrations to guide the AI image generator.

4. **Generate Illustrations**:
   - Using the Segmind SDXL model, the notebook generates images corresponding to the extracted illustration prompts.

5. **View in Gradio Interface**:
   - The final output is displayed in a Gradio-powered web UI where the story and illustrations are showcased together.

## Example Output
- **Generated Story**: A short moral story featuring different animal characters.
- **Illustrations**: AI-generated images depicting scenes from the story.
- **Interactive UI**: A simple webpage where users can read the story and view illustrations.

## Customization
- **Story Structure**: Modify the `story_prompt` to change the story format or add additional constraints.
- **Illustration Style**: Adjust the `style` variable (`"kawaii"`, `"watercolor"`, etc.) to generate illustrations in different artistic styles.
- **Number of Illustrations**: Modify `image_count` to change the number of images generated per story.

## License
This project is open-source and available under the MIT License.

## Acknowledgments
- OpenAI for GPT-3.5-turbo-16k
- Segmind for AI-powered image generation
- Gradio for the interactive UI framework
- Jupyter Notebook for providing a seamless development environment

---
This README provides a comprehensive guide to using and modifying the StoryForge - Intelligent Storytelling Assistant. Feel free to expand upon it based on future enhancements!

