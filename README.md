# 🎨 GenAI Storyline

An end-to-end multimodal AI pipeline that transforms spoken stories into illustrated children's storybooks using state-of-the-art generative AI models.

The pipeline automatically:
- 🎙️ Transcribes speech into English
- 📖 Rewrites the narration into a child-friendly story
- 🎬 Splits the story into visual scenes
- 🖼️ Generates Ghibli-style illustrations for each scene
- 📄 Exports the generated story and metadata

---

## 🚀 Pipeline

```
Audio Input
      │
      ▼
Whisper
(Speech → English Text)
      │
      ▼
Llama 3.2
Story Generation
      │
      ▼
Scene Extraction
      │
      ▼
Visual Prompt Generation
      │
      ▼
Stable Diffusion
(Image Generation)
      │
      ▼
Story + Illustrations + JSON Output
```

---

## ✨ Features

- Automatic speech transcription using OpenAI Whisper
- Story simplification for children
- Scene segmentation
- Prompt engineering for image generation
- Ghibli-style image synthesis
- JSON metadata export
- GPU-accelerated inference

---

## 🛠 Tech Stack

| Category | Tools |
|----------|-------|
| Language | Python |
| Speech Recognition | Whisper |
| LLM | Llama 3.2 3B Instruct |
| Image Generation | Stable Diffusion (Ghibli Diffusion) |
| Framework | Hugging Face Transformers |
| Deep Learning | PyTorch |
| Development | Google Colab |

---

## 📂 Project Structure

```
GenAI_storyline/

├── GenAI_storyline.ipynb
├── README.md
├── requirements.txt
├── sample_output/
│   ├── scene_1.png
│   ├── scene_2.png
│   └── output.json
└── assets/
```

---

## ⚙️ How It Works

### 1. Speech Recognition

The pipeline accepts an audio file and uses **Whisper** to transcribe and translate it into English.

### 2. Story Generation

Llama 3.2 rewrites the transcript into a simple children's story.

### 3. Scene Extraction

The generated story is divided into two meaningful scenes.

### 4. Visual Prompt Generation

Each scene is summarized into a concise visual prompt suitable for image generation.

### 5. Image Generation

Stable Diffusion generates Ghibli-inspired illustrations for each scene.

### 6. Output Generation

The pipeline produces:

- Complete story
- Scene descriptions
- Generated illustrations
- JSON metadata

---

## 📦 Output

```
output/

├── scene_1.png
├── scene_2.png
└── output.json
```

---

## 📸 Example Workflow

```
Audio Story
      ↓
English Transcript
      ↓
Children's Story
      ↓
Scene 1 + Scene 2
      ↓
Visual Prompts
      ↓
Generated Illustrations
```

---

## 🔧 Installation

```bash
git clone https://github.com/C0d3rV/GenAI_storyline.git

cd GenAI_storyline

pip install -r requirements.txt
```

---

## ▶️ Run

Open the notebook in Google Colab and execute all cells.

Make sure to:

- Add your Hugging Face access token as a Colab Secret (`HF_TOKEN`)
- Enable GPU runtime
- Provide an input audio file

---

## 🔮 Future Improvements

- Generate animated story videos
- Support multiple languages
- Produce narrated audiobooks
- Interactive story editing
- Longer stories with dynamic scene generation
- Character consistency across illustrations

---

## 📜 License

This project is released under the MIT License.
