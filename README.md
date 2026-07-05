# Multimodal AI Design Agent Team

A sophisticated Streamlit application that leverages multiple AI agents to provide comprehensive design analysis using multimodal AI capabilities.

## Features

- **Visual Design Analysis** - Analyzes design elements, color schemes, typography, layouts, and visual hierarchy
- **UX Analysis** - Evaluates user flows, interaction patterns, usability, and accessibility
- **Market Analysis** - Conducts market research, identifies trends, and suggests positioning opportunities
- **Multi-File Support** - Process multiple designs and competitor designs simultaneously
- **Image Processing** - Upload and analyze high-resolution UI/UX design images

## Architecture

The application uses a team of specialized AI agents:

1. **Vision Agent** - Analyzes visual design elements and patterns
2. **UX Agent** - Evaluates user experience and interaction design
3. **Market Agent** - Conducts market research and competitive analysis (with web search capabilities)

## Requirements

- Python 3.8+
- OpenRouter API Key
- Internet connection (for market analysis web search)

## Installation

1. **Clone or download the project**
   ```bash
   cd multimodel_design_agent
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**
   - Create a `.env` file in the project root
   - Add your OpenRouter API key:
     ```
     OPENROUTER_API_KEY=your_api_key_here
     ```

## Usage

Run the Streamlit application:

```bash
streamlit run design_agent.py
```

The application will be available at `http://localhost:8501`

### Steps to Use

1. **Upload Designs** - Upload your UI/UX design files (JPG, JPEG, PNG)
2. **Optional: Add Competitors** - Upload competitor design files for comparison
3. **Configure Analysis** - Select analysis types and focus areas
4. **Add Context** - Provide additional context about your product or target audience
5. **Run Analysis** - Click the "Run Analysis" button to get AI-powered insights

## Project Structure

```
multimodel_design_agent/
├── design_agent.py          # Main application file
├── requirements.txt         # Python dependencies
├── .env                     # Environment variables (create this)
├── .env.example            # Example environment variables
├── .gitignore              # Git ignore patterns
└── README.md               # This file
```

## Dependencies

- **streamlit** - Web framework for building the UI
- **agno** - Agent framework for multi-agent orchestration
- **openai** - OpenAI client for API interactions
- **openrouter** - OpenRouter API integration
- **python-dotenv** - Environment variable management
- **duckduckgo-search** - Search functionality for market analysis

## Configuration

### Analysis Types

- Visual Design
- User Experience
- Market Analysis

### Focus Areas

- Color Scheme
- Typography
- Layout
- Navigation
- Interactions
- Accessibility
- Branding
- Market Fit

## Error Handling

The application includes comprehensive error handling:
- API key validation
- Image processing error handling
- Agent initialization error checks
- Detailed error logging

## Logging

Logging is configured to capture errors only. Check the console or logs for debugging information.

## API Keys

### Getting an OpenRouter API Key

1. Visit [OpenRouter.ai](https://openrouter.ai)
2. Sign up for an account
3. Navigate to API keys section
4. Generate a new API key
5. Add it to your `.env` file

## Performance Tips

- Use high-resolution images for better analysis
- Include multiple design screenshots for comprehensive context
- Provide specific context about your target audience
- For competitor analysis, upload similar design categories

## Troubleshooting

### "API Key not found"
- Ensure `.env` file exists in the project root
- Check that `OPENROUTER_API_KEY` is correctly set
- Restart the Streamlit application

### "Failed to initialize agents"
- Verify your OpenRouter API key is valid
- Check internet connectivity
- Review error logs for specific issues

### "ModuleNotFoundError"
- Ensure all dependencies are installed: `pip install -r requirements.txt`
- Verify you're using the correct Python environment

## Future Enhancements

- Support for additional image formats (PDF, SVG)
- Design comparison tools
- Historical analysis tracking
- Export analysis reports
- Team collaboration features
- Real-time feedback integration

## License

This project is proprietary software for Maarga Accelerated Demos.

## Support

For issues or questions, contact the development team.

## Changelog

### v1.0.0
- Initial release
- Multi-agent design analysis
- Visual, UX, and market analysis
- Image processing and upload functionality
