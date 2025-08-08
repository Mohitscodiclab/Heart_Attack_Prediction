# Heart Disease Prediction Web Application

![Heart Disease Predictor](https://img.shields.io/badge/Status-Active-brightgreen) ![Technology](https://img.shields.io/badge/Technology-HTML%2FCSS%2FJS-blue) ![License](https://img.shields.io/badge/License-MIT-green)

A comprehensive web application for predicting heart disease risk using advanced AI algorithms. This application runs entirely in the browser without requiring any server-side processing, storing all data locally.

## Demo

Check out the live demo: [Use Only for Educational Purpose](https://mohitscodiclab.github.io/Heart_Attack_Prediction/)

## Features

- **User-Friendly Interface**: Clean, modern design with intuitive navigation
- **Dual Mode Operation**:
  - Basic Mode: Simple interface for general users with 9 common risk factors
  - Advanced Mode: Clinical interface with 14 parameters for healthcare professionals
- **Advanced Neural Network**: AI model trained on 10,000+ synthetic patient records
- **Factor Impact Analysis**: Detailed breakdown of how each factor contributes to risk
- **Local Storage**: All predictions saved locally with complete history
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **No Server Required**: Runs entirely in the browser using client-side technologies

## Technology Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **AI Model**: Custom neural network implementation
- **Data Storage**: Browser's LocalStorage API
- **UI Framework**: Custom CSS with responsive design
- **Deployment**: GitHub Pages

## How to Use

1. **Basic Mode** (Default):
   - Enter patient information including age, gender, vital signs, and lifestyle factors
   - Click "Predict Risk" to get an instant assessment
   - View detailed results with risk percentage and factor analysis

2. **Advanced Mode**:
   - Enable "Advanced Mode (for clinical use)" checkbox
   - Additional clinical parameters will appear:
     - Chest Pain Type
     - Resting ECG Results
     - ST Depression (mm)
     - Number of Major Vessels (0-3)
     - Thalassemia
   - Fill in the additional parameters for more accurate prediction
   - Results will include analysis of all factors

3. **History**:
   - Switch to the "History" tab to view past predictions
   - Each prediction shows patient name, date, and risk level
   - Option to clear history when needed

## Project Structure

```
Heart_Attack_Prediction/
├── index.html          # Main application file
├── assets/             # Images and other assets (if any)
└── README.md           # This file
```

## Advanced Mode

The Advanced Mode provides additional clinical parameters that significantly improve prediction accuracy:

- **Chest Pain Type**: Differentiates between typical angina, atypical angina, non-anginal pain, and asymptomatic cases
- **Resting ECG Results**: Identifies ST-T wave abnormalities and left ventricular hypertrophy
- **ST Depression**: Measures ST segment depression in millimeters, a key indicator of ischemia
- **Major Vessels**: Number of major vessels colored by fluoroscopy (0-3)
- **Thalassemia**: Blood disorder status (normal, fixed defect, reversible defect)

These parameters are particularly valuable for healthcare professionals conducting clinical assessments.

## Model Details

The application uses a neural network with the following architecture:

- **Input Layer**: 14 neurons (9 in basic mode, 14 in advanced mode)
- **Hidden Layer**: 20 neurons with sigmoid activation
- **Output Layer**: 1 neuron with sigmoid activation (probability of heart disease)

The model was trained on a synthetic dataset of 10,000+ patient records with the following features:
- Age, gender, blood pressure, cholesterol, blood sugar
- Maximum heart rate, exercise-induced angina
- Smoking status, family history
- Chest pain type, resting ECG results
- ST depression, number of major vessels, thalassemia

Feature normalization is applied to continuous variables for better model performance.

## Future Enhancements

- Integration with real medical datasets
- Export functionality for prediction reports
- Multi-language support
- Additional visualization of risk factors over time
- Integration with wearable devices for real-time monitoring
- Doctor referral system based on risk level

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Disclaimer

This application is for educational and informational purposes only. It is not a substitute for professional medical advice, diagnosis, or treatment. Always seek the advice of your physician or other qualified health provider with any questions you may have regarding a medical condition.

## Acknowledgments

- The neural network model was inspired by research on heart disease prediction
- UI design follows modern web accessibility standards
- Thanks to all contributors who helped improve this application
