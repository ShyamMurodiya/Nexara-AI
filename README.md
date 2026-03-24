# PredictiveAI - Maintenance Intelligence

PredictiveAI is an AI-powered predictive maintenance scheduling application designed for manufacturing equipment. Built with Python and Streamlit, this application helps detect degradation patterns, identify near-misses, and generate maintenance schedules using both rule-based heuristics and advanced machine learning techniques.

## Features

- 📈 **Degradation Pattern Detection**: Identify temperature, vibration, and pressure anomalies from equipment logs.
- ⚠️ **Near-Miss Detection**: Spot parameters that are approaching critical thresholds before failures occur.
- 📅 **Confidence-Based Scheduling**: Generate maintenance schedules prioritized with confidence scores.
- 🤖 **Multi-LLM Chat Assistant**: Chat with 5 different AI providers (OpenAI, Anthropic, Gemini, Groq, Cohere) for intelligent log analysis.
- 🔬 **ML Anomaly Detection**: Uncover hidden anomalies using the Isolation Forest algorithm.
- 📊 **Failure Prediction**: Estimate machine failure probability using Machine Learning.
- 📄 **Report Export**: Download comprehensive maintenance reports as DOCX files.
- 📊 **Data Explorer & Interactive Dashboards**: Explore interactive visualizations built with Plotly.

## Installation

1. Clone or download the repository.
2. (Optional) Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Configuration

To enable the AI-powered analysis features, you will need to provide your API keys. The application supports multiple LLM providers.



## Usage

Start the Streamlit application by running:

```bash
streamlit run app.py
```

Once the application is running, you can:
1. Upload your equipment log CSV file via the sidebar.
2. Alternatively, click **"Load Sample Data"** to try out the application with the included sample dataset (`dataset/sample_logs.csv`).
3. Explore the various tabs including Dashboard, Patterns, Near-Misses, Schedule, ML Anomaly Detection, and the Multi-LLM Chat Assistant.

## Project Structure

- `app.py`: The main Streamlit dashboard application.
- `ai_engine.py`: Handles integrations with various LLM providers for data analysis and the chat assistant.
- `ml_features.py`: Contains machine learning models for anomaly detection and failure prediction.
- `pattern_detector.py`: Implements rule-based heuristics for degradation pattern and near-miss detection.
- `llm_provider.py`: Utility module for managing LLM clients.
- `dataset/`: Contains sample data for demonstration.
- `.env.example`: Template for environment variables.
- `requirements.txt`: Python package dependencies.

## License

This project is licensed under the MIT License.
