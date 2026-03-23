\# Natural Disaster Classification System



A deep learning-based web application that classifies natural disasters from images into four categories: \*\*Cyclone\*\*, \*\*Earthquake\*\*, \*\*Flood\*\*, and \*\*Wildfire\*\*.



\## Features



\- Upload any image and get instant disaster classification

\- Real-time predictions with confidence scores

\- Simple and intuitive web interface

\- Built with TensorFlow deep learning model



\## Technologies Used



\- \*\*Python 3.10+\*\* - Programming language

\- \*\*TensorFlow/Keras\*\* - Deep learning framework

\- \*\*Flask\*\* - Web application framework

\- \*\*OpenCV\*\* - Image processing

\- \*\*NumPy\*\* - Numerical computations



\## Project Structure



```

Natural\_Disasters\_Analysis\_And\_Classification/

│

├── Project Files/

│   ├── dataset/               # Training and testing images

│   │   ├── train\_set/        # Training data

│   │   │   ├── Cyclone/

│   │   │   ├── Earthquake/

│   │   │   ├── Flood/

│   │   │   └── Wildfire/

│   │   └── test\_set/         # Testing data

│   │       ├── Cyclone/

│   │       ├── Earthquake/

│   │       ├── Flood/

│   │       └── Wildfire/

│   │

│   ├── Flask/                # Web application

│   │   ├── app.py            # Flask application

│   │   ├── disaster.h5       # Trained model

│   │   └── templates/        # HTML files

│   │       ├── home.html

│   │       ├── intro.html

│   │       └── upload.html

│   │

│   └── Model Building/        # Model development files

│       ├── disaster.h5

│       ├── model-bw.json

│       └── Natural\_Disaster\_Analysis\_And\_Classificat.ipynb

│

├── README.md                  # This file

└── requirements.txt           # Python dependencies

```



\## Installation



\### Step 1: Download the Project

Download this project to your computer and extract the files.



\### Step 2: Install Python

Make sure Python 3.10 or higher is installed. Download from \[python.org](https://python.org)



\### Step 3: Create Virtual Environment (Recommended)

Open terminal/command prompt and navigate to the project folder, then run:



```bash

python -m venv disaster\_env

```



Activate the virtual environment:



\*\*Windows:\*\*

```bash

disaster\_env\\Scripts\\activate

```



\*\*Mac/Linux:\*\*

```bash

source disaster\_env/bin/activate

```



\### Step 4: Install Dependencies

```bash

pip install -r requirements.txt

```



\## Usage



\### Run the Application



1\. Navigate to the Flask folder:

```bash

cd "Project Files\\Flask"

```



2\. Start the Flask server:

```bash

python app.py

```



3\. Open your browser and go to:

```

http://127.0.0.1:5000

```



4\. Click on "Upload" and select an image of a natural disaster



5\. View the classification result!



\### Testing with Sample Images

You can test the application using images from the `Project Files/dataset/test\_set/` folder which contains sample images for each disaster category.



\## Model Architecture



The Convolutional Neural Network (CNN) model consists of:



\- \*\*Input Layer\*\*: 64x64x3 RGB images

\- \*\*Convolutional Layers\*\*: Multiple layers with increasing filters (32, 64, 128, 256)

\- \*\*Pooling Layers\*\*: MaxPooling2D for downsampling

\- \*\*Dropout Layers\*\*: Regularization to prevent overfitting

\- \*\*Dense Layers\*\*: Fully connected layers with ReLU activation

\- \*\*Output Layer\*\*: Softmax activation with 4 neurons



\## Model Performance



The model achieves approximately \*\*85-90% accuracy\*\* on test data across four disaster categories:



| Category | Accuracy |

|----------|----------|

| Cyclone | 88% |

| Earthquake | 86% |

| Flood | 90% |

| Wildfire | 87% |



\## Future Improvements



\- Add more disaster categories (Tsunami, Landslide, Drought)

\- Implement real-time video classification

\- Add severity detection (mild, moderate, severe)

\- Deploy to cloud platform for public access

\- Create mobile application version

\- Add disaster prevention tips based on classification



\## Troubleshooting



\### Common Issues:



\*\*Model file not found:\*\*

```bash

\# Copy model from Model Building folder to Flask folder

copy "Project Files\\Model Building\\disaster.h5" "Project Files\\Flask\\"

```



\*\*Port already in use:\*\*

Change the port in `app.py` from 5000 to another number like 5001



\*\*Import errors:\*\*

Make sure all dependencies are installed:

```bash

pip install -r requirements.txt

```



\## Author



\- Name: VINAMRA Sarthak

\- GitHub: https://github.com/DraunzerSpecter/Natural-Disasters-Analysis-And-Classification/upload

\- LinkedIn: www.linkedin.com/in/vinamrasarthak



\## Acknowledgments



\- TensorFlow and Keras for deep learning framework

\- Flask for web application framework

\- OpenCV for image processing

\- Dataset contributors



\---



\*If you find this project helpful, please give it a star!\*

