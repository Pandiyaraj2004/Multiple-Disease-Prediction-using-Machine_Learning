# Multiple Disease Prediction

> An educational Flask application combining tabular machine-learning models and image classifiers in one interface.

**Python · Flask · scikit-learn · TensorFlow/Keras · NumPy · Pillow**

## Project overview

The application loads saved models and exposes separate web forms for different prediction tasks. It demonstrates how model artifacts, preprocessing, server routes, and HTML templates fit together in an inference application.

| Input | Implemented tasks | Model format |
| --- | --- | --- |
| Numeric form fields | Diabetes, breast cancer, heart, kidney, liver | Pickle (`.pkl`) |
| Uploaded images | Malaria, pneumonia | Keras (`.h5`) |

## Engineering highlights

- Routes for seven task-specific interfaces.
- Numeric input conversion and dispatch to the corresponding tabular model.
- Separate image preprocessing for RGB malaria images and grayscale pneumonia images.
- Saved model artifacts and five tabular-model notebooks included in the repository.

## Repository guide

| Path | Contents |
| --- | --- |
| [app.py](app.py) | Routes, preprocessing, model loading, predictions |
| [models](models) | Serialized classifiers |
| [Python Notebooks](Python%20Notebooks) | Tabular-model experimentation |
| [templates](templates) | Input forms and result pages |
| [requirements.txt](requirements.txt) | Original pinned dependencies |

## Reproducing the application

```bash
git clone https://github.com/Pandiyaraj2004/Multiple-Disease-Prediction-using-Machine_Learning.git
cd Multiple-Disease-Prediction-using-Machine_Learning
python -m pip install -r requirements.txt
python app.py
```

Open http://localhost:5000 after dependencies and models load successfully.

**Compatibility:** this is a legacy environment. `runtime.txt` specifies Python 3.6.8, and the dependency list contains older TensorFlow and scikit-learn releases. A fresh installation on a current Python version is not verified. Reproduce in an isolated compatible environment, or update dependencies and revalidate/retrain the saved models together.

## Evaluation and intended use

This repository is an educational demonstration, not a clinically validated diagnostic system. No accuracy percentage or medical effectiveness is asserted here. Use synthetic or appropriately de-identified examples, and review the training notebooks before drawing conclusions about model performance.

---

Built by **Pandiyaraj A** · [Portfolio](https://pandiyaraj.netlify.app/) · [GitHub](https://github.com/Pandiyaraj2004) · [LinkedIn](https://www.linkedin.com/in/pandiyaraj-a-mca/)
