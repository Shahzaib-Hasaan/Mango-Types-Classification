# Mango Types Classifier 🥭

Computer vision app that classifies mango varieties from a photo. Classical CV pipeline (no deep learning): hand-crafted image features + a scikit-learn classifier, wrapped in a Streamlit web UI.

Part of my BS Artificial Intelligence degree work.

## How it works

1. Upload a mango image in the Streamlit app
2. The image is resized and converted, then features are extracted with **scikit-image** (color + texture descriptors)
3. A pre-trained scikit-learn model (loaded via joblib) predicts the mango variety

The point of the project: you don't always need a GPU and a CNN — classical features + a lightweight classifier run instantly on CPU and are fully explainable.

## Run it

```bash
pip install -r requirements.txt
streamlit run main.py
# open http://localhost:8501
```

## Stack

`Python` `Streamlit` `scikit-image` `scikit-learn (joblib model)` `NumPy` `Pillow`

---

More of my work: [shahzaibbuilds.me](https://shahzaibbuilds.me) · [LinkedIn](https://www.linkedin.com/in/shahzaib-hassan-ai-developer/)
