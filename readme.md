# Supercharge Your Agents with Heroku

A simple, interactive web application that showcases various ways to enhance your agents' capabilities using Heroku's computational power. The application features an expandable interface with detailed information about different use cases for Heroku integration.

## Features

- Responsive design with a clean, modern interface
- Interactive expandable/collapsible sections
- Custom styling with Heroku's brand colors
- Mobile-friendly layout
- Seven key topics covering different aspects of agent enhancement:
  - Advanced Data Analysis
  - Real-time Decision Making
  - Personalized Recommendations
  - Generative Content Creation
  - Scientific Modeling and Simulation
  - Natural Language Processing (NLP) Advancements
  - Computer Vision Applications

## Local Development

1. Clone this repository:
```bash
git clone <your-repository-url>
cd <repository-name>
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

3. Install the required dependencies:
```bash
pip install -r requirements.txt
```

4. Run the application locally:
```bash
python -m http.server 8000
```

5. Open your web browser and navigate to `http://localhost:8000`

## Deployment to Heroku

### Prerequisites

1. [Create a Heroku account](https://signup.heroku.com/) if you haven't already
2. Install the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli)
3. Install [Git](https://git-scm.com/downloads) if you haven't already

### Deployment Steps

1. Login to Heroku CLI:
```bash
heroku login
```

2. Create a new Heroku app:
```bash
heroku create your-app-name
```

3. Ensure you have the following files in your project root:
   - `requirements.txt` - Contains: `Flask==2.3.2`
   - `Procfile` - Contains: `web: python -m http.server $PORT`
   - `index.html`

4. Initialize a Git repository (if not already done):
```bash
git init
```

5. Add your files:
```bash
git add .
git commit -m "Initial commit"
```

6. Push to Heroku:
```bash
git push heroku main
```

7. Open your deployed application:
```bash
heroku open
```

## Project Structure

```
root/
├── index.html         # Main application file with HTML, CSS, and JavaScript
├── Procfile          # Heroku deployment configuration
├── requirements.txt  # Python dependencies
└── venv/            # Virtual environment (not tracked in Git)
```

## Technical Details

- Python-based server using `http.server`
- Pure HTML/CSS/JavaScript frontend
- No external frontend dependencies required
- Uses CSS animations for smooth transitions
- Inline styles and scripts for simplicity

## Environment Variables

The application uses the following environment variables:
- `PORT` - Automatically set by Heroku for serving the application

## License

This project is open source and available under the MIT License.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

## Support

For any questions or issues, please open an issue in the repository or contact the development team.