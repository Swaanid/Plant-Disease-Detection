

# Plant Disease Detection

This project is a Flask-based web application designed to detect plant diseases using a pre-trained deep learning model. Users can upload images of plant leaves to classify the disease and view results interactively.

---

## Features

1. **Image Upload**: Allows users to upload an image of a plant leaf.
2. **Disease Detection**: Predicts the disease class and displays confidence scores.
3. **Interactive UI**: Includes a clean, intuitive HTML interface styled with CSS.
4. **Pre-trained Model**: Utilizes a robust `.keras` model trained using transfer learning.

---

## Project Structure

```
Plant Detection/
├── static/
│   ├── styles.css            # CSS for styling the web interface
│   └── uploads/              # Folder for storing uploaded images
├── templates/
│   └── index.html            # HTML template for the web interface
├── detection.py              # Flask app handling uploads and predictions
├── model_training.ipynb      # Jupyter Notebook for training the model
├── model/
│   └── my_model_2.keras      # Trained model file
├── requirements.txt          # Python dependencies
└── README.md                 # Documentation
```

---

## Prerequisites

- Python 3.8 or later
- A virtual environment (optional but recommended)
- Required libraries listed in `requirement.txt`

Install dependencies using:
```bash
pip install -r requirement.txt
```

---

## Setup and Usage

### 1. Clone the Repository

```bash
git clone https://github.com/Swaanid/Plant-Disease-Detection.git
cd Plant-Detection-Detection
```

### 2. Download the Model

The trained model file (`my_model_2.keras`) is too large to be included in the repository. It must be downloaded separately:

1. Download the model file from [Google Drive](https://drive.google.com/file/d/1c3Yyca_QZKQ2jaV1cJFXDfWCp-iyzes7/view?usp=sharing).
2. Place it in the `model/` directory. Create the directory if it doesn't exist.

### 3. Run the Application

Start the Flask server:

```bash
python detection.py
```

Access the application at [http://127.0.0.1:5000](http://127.0.0.1:5000).

---

## Usage Instructions

1. Navigate to the web application in your browser.
2. Upload an image of a plant leaf using the provided form.
3. View the prediction results, including the detected disease and confidence score.

---

## Training the Model

- The model was trained using the `training.ipynb` Jupyter Notebook.
- The training process includes:
  - Data augmentation (shearing, zooming, horizontal flips)
  - Image resizing to `(128, 128)`
  - Model saving in `.keras` format

---

## File Details

- **`detection.py`**: Handles the Flask server, image upload, and prediction logic.
- **`training.ipynb`**: Includes code for training the deep learning model.
- **`index.html`**: Front-end interface for uploading images.
- **`style.css`**: Adds styling to the HTML interface.

---

## Common Issues

1. **Model Not Found**:
   - Ensure the model file is downloaded and placed in the correct directory (`model/my_model_2.keras`).

2. **Dependency Errors**:
   - Ensure all required libraries are installed via `requirements.txt`.

3. **Google Drive Access**:
   - Ensure the file link is publicly accessible if using Google Drive to host the model.

---

## License

This project is licensed under the MIT License.

---

Let me know if you want any further customization!
