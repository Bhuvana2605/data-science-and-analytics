# 🧠 Image Captioning + Segmentation Project

This project combines **Image Captioning** and **Image Segmentation** into a single pipeline using **pretrained deep learning models**. It is designed to give a hands-on introduction to the intersection of **Computer Vision (CV)** and **Natural Language Processing (NLP)**.

---

## 🚀 Features

- 📷 Upload any image (via Google Colab)
- 📝 Generate descriptive captions using BLIP (Transformer-based model)
- 🧩 Perform semantic segmentation using DeepLabV3 (ResNet-101 backbone)
- 🎨 Visualize the original image, generated caption, and segmented image
- ✅ Runs fully in Google Colab – no local setup required

---

## 📦 Tech Stack

- **Python**
- **PyTorch** (for segmentation)
- **Hugging Face Transformers** (for captioning)
- **OpenCV / PIL** (image handling)
- **Google Colab** (runtime environment)
- **MS COCO / Pascal VOC** (used via pretrained models)

---

## 📁 File Structure

```
.
├── Image_Captioning_Segmentation.ipynb   # Colab notebook with code and markdown
├── sample_images/                         # Optional test images
├── README.md                              # This file
```

---

## 📋 How to Run in Colab

1. Open [Google Colab](https://colab.research.google.com)
2. Upload `Image_Captioning_Segmentation.ipynb`
3. Run each cell in sequence:
   - Install libraries
   - Upload an image
   - Generate caption
   - Perform segmentation
4. View output: caption text and segmented image

---

## 🤖 Models Used

### 📝 Image Captioning

- **Model**: [BLIP base](https://huggingface.co/Salesforce/blip-image-captioning-base)
- **Trained on**: MS COCO
- **Library**: Hugging Face Transformers

### 🧩 Image Segmentation

- **Model**: DeepLabV3 (ResNet-101 backbone)
- **Trained on**: Pascal VOC 2012
- **Library**: PyTorch torchvision

---

## ✅ Sample Output

| Original Image | Caption                | Segmentation      |
| -------------- | ---------------------- | ----------------- |
| 🖼️ Uploaded   | "A man riding a horse" | 🎨 Segmented mask |

---

## 📝 Summary

This project demonstrates the integration of vision and language using two state-of-the-art pretrained models. It is ideal for beginners or interns looking to get started with practical computer vision and NLP without needing to train models from scratch.

---

## 📌 Future Work

- Training models from scratch using COCO/VOC datasets
- Model evaluation using BLEU, IoU metrics
- Web-based deployment using Streamlit or Gradio

---

## 🔗 Credits

- [Hugging Face](https://huggingface.co/)
- [PyTorch](https://pytorch.org/)
- [COCO Dataset](https://cocodataset.org/)
- [PASCAL VOC Dataset](http://host.robots.ox.ac.uk/pascal/VOC/)

---

## 📄 License

MIT License

