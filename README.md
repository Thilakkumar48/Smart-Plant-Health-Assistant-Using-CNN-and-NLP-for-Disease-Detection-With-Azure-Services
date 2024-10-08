# Smart-Plant-Health-Assistant-Using-CNN-and-NLP-for-Disease-Detection-With-Azure-Services


This application helps classify plant diseases using Azure Custom Vision and provides disease diagnosis based on symptoms entered by the user. It also supports translating the diagnosis into multiple languages and converting it to speech using Azure services.

## Features

1. **Plant Disease Classification**:
   - Upload an image of a plant, and the app will predict the disease using Azure Custom Vision.
   
2. **Disease Diagnosis**:
   - Input plant symptoms to receive a possible diagnosis generated by Azure OpenAI (GPT-3.5).
   
3. **Translation**:
   - Translate the diagnosis into multiple languages using Azure Translator.
   
4. **Text-to-Speech**:
   - Listen to the translated diagnosis using Azure Speech Service.

## Tech Stack

- **Frontend**: Streamlit
- **Backend**: Python
- **Azure Services**:
  - Custom Vision for plant disease classification
  - OpenAI for disease diagnosis generation
  - Translator API for language translation
  - Speech API for converting text to speech

## Setup

### Prerequisites

- Python 3.8+
- Azure Custom Vision setup
- Azure Translator API
- Azure Speech Service
- Azure OpenAI setup

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Thilakkumar48/Plant-Disease-Assistant.git
   cd Plant-Disease-Assistant
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Azure Configuration

You will need to set up your Azure services and obtain the necessary API keys.

- **Custom Vision API**: 
  - Obtain the `Prediction Key` and `Endpoint` from your Azure Custom Vision service.
  - Replace the `prediction_key`, `endpoint`, and `project_id` values in the code.
  
- **OpenAI API**:
  - Set up Azure OpenAI and obtain the `API Key` and `Endpoint`.
  - Replace the `openai_api_key` and `openai_endpoint` values in the code.

- **Translator API**:
  - Obtain the Translator API key and region from Azure Translator service.
  - Replace the `translator_key` and `translator_endpoint` in the code.

- **Speech Service API**:
  - Get the Speech API key and region from the Azure Speech service.
  - Replace `speech_key` and `speech_region` in the code.

### How to Run

1. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

2. Open the browser to interact with the application. You can upload a plant image, enter symptoms, get a diagnosis, and translate/speak the diagnosis.

### Using the App

1. **Upload Plant Image**: Upload an image of the plant, and the app will classify the disease using Custom Vision.
2. **Disease Diagnosis**: Input plant symptoms (or use the predicted disease name from the image classification) and get a diagnosis using OpenAI.
3. **Translation and Speech**: Choose languages, translate the diagnosis, and listen to the diagnosis in different languages using Azure Speech.

### Future Improvements

- Adding more supported languages for translation and speech.
- Enhancing the model's disease classification by training on more images.
- Adding more detailed information on the predicted diseases and suggestions for treatment.

---

### Author

- **Thilak Kumar K**  
  - GitHub: [Thilakkumar48](https://github.com/Thilakkumar48)

```

This `README.md` file provides a clear structure for understanding and setting up the application.
