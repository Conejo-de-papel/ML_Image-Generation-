# Image Generation with Hugging Face API

This project allows you to generate images using the **Stable Diffusion** model via the Hugging Face API. The application is built with Python and uses the `gradio` library to provide a user-friendly interface.

## Features

- Generate images from text prompts.
- Customize image generation with parameters like:
  - **Negative Prompt**: Specify what you don't want in the image.
  - **Inference Steps**: Control the number of steps for image generation.
  - **Guidance Scale**: Adjust the creativity vs. adherence to the prompt.
  - **Width and Height**: Set the dimensions of the generated image.
- Simple and intuitive interface powered by Gradio.

---

## Installation

Follow these steps to set up the project locally:

1. **Clone the repository**:
   ```bash
   git clone [https://github.com/your-username/your-repo-name.git](https://github.com/Conejo-de-papel/ML_Image-Generation-)
   cd your-repo-name
   ```

2. **Install dependencies**:
   Make sure you have Python 3.8+ installed. Then, install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up your Hugging Face API key**:
   - Create a `.env` file in the project root directory.
   - Add your Hugging Face API key to the `.env` file:
     ```
     HF_API_KEY=your_hugging_face_api_key_here
     ```
   - **Note**: Do not share your API key publicly. Add `.env` to your `.gitignore` file to avoid committing it to the repository.

4. **Run the application**:
   ```bash
   python app.py
   ```

5. **Access the application**:
   - The application will launch locally, and you can access it in your browser at `http://127.0.0.1:7860`.
   - If you want to share the app publicly, use the `share=True` option in `demo.launch()`.

---

## Usage

1. Enter a **text prompt** describing the image you want to generate.
2. (Optional) Provide a **negative prompt** to specify what you don't want in the image.
3. Adjust the parameters:
   - **Inference Steps**: More steps can improve quality but take longer.
   - **Guidance Scale**: Higher values make the image adhere more closely to the prompt.
   - **Width and Height**: Set the dimensions of the output image.
4. Click **Submit** to generate the image.
5. View the generated image in the output section.

---

## Example Prompts

- **Prompt**: "A futuristic cityscape at sunset, cyberpunk style, neon lights, highly detailed"
- **Negative Prompt**: "blurry, low quality, distorted"
- **Inference Steps**: 30
- **Guidance Scale**: 7.5
- **Width**: 512
- **Height**: 512

---

## Dependencies

- Python 3.8+
- Libraries:
  - `requests`: For making API calls to Hugging Face.
  - `gradio`: For building the user interface.
  - `Pillow`: For image processing.
  - `python-dotenv`: For loading environment variables.

You can install all dependencies using:
```bash
pip install -r requirements.txt
```


