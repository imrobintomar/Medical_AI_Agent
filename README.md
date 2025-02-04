# 🏥 AI Medical History Assistant

An intelligent medical history management system powered by AI that helps healthcare professionals track and manage patient histories through natural conversation.

## Features

- **Secure Login System**: Protected access with username/password authentication
- **Patient ID Validation**: Enforces standardized patient ID format (PAT-XXXXX)
- **Intelligent Chat Interface**: Natural conversation with context-aware responses
- **Memory Management**: Remembers previous interactions and medical history
- **Synthetic Data Generation**: Create realistic patient profiles for testing
- **Real-time Patient Profile View**: Quick access to comprehensive patient information

## Prerequisites

- Python 3.8+
- Streamlit
- OpenAI API key
- Qdrant vector database (running locally or remote)
- Other dependencies listed in `requirements.txt`

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ai-medical-history-assistant.git
cd ai-medical-history-assistant
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Set up environment variables:
Create a `.env` file in the root directory with:
```
OPENAI_API_KEY=your_openai_api_key_here
```

4. Start the Qdrant vector database:
```bash
docker run -p 6333:6333 qdrant/qdrant
```

## Usage

1. Start the application:
```bash
streamlit run main.py
```

2. Login with default credentials:
   - Username: admin
   - Password: admin

3. Enter a patient ID (format: PAT-XXXXX)

4. Generate synthetic data or view existing patient profiles

5. Start chatting with the AI assistant about the patient's medical history

## Key Components

- `MedicalHistoryAgent`: Manages interactions with OpenAI API and memory storage
- `Memory`: Handles vector storage and retrieval of patient information
- `manage_sidebar`: Controls patient profile management and synthetic data generation
- `chat_interface`: Manages the chat UI and message history

## Security Notice

This is a demonstration version with basic security features. For production use:
- Implement proper user authentication
- Use secure password storage
- Enable encryption for sensitive data
- Follow relevant healthcare data protection regulations (HIPAA, etc.)

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- OpenAI for providing the GPT API
- Streamlit for the web interface framework
- Qdrant for vector storage capabilities
- All contributors and testers

## Support

For support, please open an issue in the GitHub repository or contact us at itsrobintomar@gmail.com.
