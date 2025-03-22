# DeepLearningImage

# 🧠 Image Classifier with VGG16 (No API Needed)

## 📌 Overview
This project uses the **pretrained VGG16 model** from Keras to classify images into top-3 ImageNet categories. It’s built to run seamlessly on **Google Colab**, requires **no API keys**, and features a sleek, interactive **Gradio UI** for image upload and prediction.

---

## 🛠️ Tech Stack
| Task                  | Tool/Library |
|-----------------------|--------------|
| Deep Learning Model   | VGG16 (Keras) |
| Image Processing      | TensorFlow / Keras |
| Web UI                | Gradio |
| Environment           | Google Colab |

---

## 💡 Features
- ✅ Upload your own image for classification
- ✅ Predicts top 3 labels from ImageNet
- ✅ Visual + textual output
- ✅ Beginner-friendly, no login or API setup

---

## 🖼️ Sample Output
Upload an image → Get predictions like:
```
mask: 12.18%
toyshop: 11.62%
sunglasses: 11.34%
```

---

## 🌐 Gradio Interface (Live Demo)
No code needed. Just upload your image and get the top 3 predictions instantly with confidence scores.

```python
# Sample Gradio Setup
import gradio as gr

def predict_image(img_path):
    ... # full prediction code

gr.Interface(
    fn=predict_image,
    inputs=gr.Image(type="filepath"),
    outputs=["image", "text"]
).launch(share=True)
```

---

## 🔮 Future Scope
- Replace VGG16 with ResNet or EfficientNet
- Train on your own dataset
- Add class activation maps (CAMs) to highlight focus areas

---
---
---

Made with ❤️ by [Ishita Vasishth](https://github.com/ishitavasishth)

