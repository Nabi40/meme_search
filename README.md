## meme_search  
**OpenAI CLIP · Vision-Language Model · Image Search**  

This project demonstrates a simple image search engine using OpenAI's **CLIP** model.  
It allows you to input a natural language query (e.g., *"girl crying"*) and returns the most relevant meme image based on semantic similarity.

---

## 📌 How It Works

### 1. Download Memes  
- Downloads 5 meme images from a remote server  
- Saves them in the `content/memes/` directory

### 2. Display Memes  
- Loads and displays all meme images using `PIL.Image`  
- Resizes for consistent visualization

### 3. Load CLIP Model  
- Loads the `ViT-B/32` variant of OpenAI’s CLIP  
- Uses `clip.load()` and detects GPU or CPU

### 4. Preprocess Images  
- Filters for supported image types  
- Preprocesses each image into tensors using CLIP's preprocessing pipeline

### 5. Search by Text  
- Tokenizes the user’s query  
- Encodes both the query and images with CLIP  
- Computes cosine similarity between the text and image features  
- Returns and displays the most relevant image

---

## 📌 Features

- ✅ Semantic image search with natural language  
- 🤖 Powered by OpenAI’s CLIP model (`ViT-B/32`)  
- 🖼️ Displays all valid meme images  
- 🔍 Top-1 most relevant result shown automatically  
- 🚫 Skips corrupt/unreadable images

---

## ❌ Limitations

- 🔸 Only searches among 5 hardcoded meme images  
- 🔸 Only shows the single best match (no ranked list)  
- 🔸 No GUI — runs entirely within Jupyter Notebook  
- 🔸 Not integrated with any external search engine or meme database

---

## 📁 Directory Structure

