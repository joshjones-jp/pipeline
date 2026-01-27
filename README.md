# Pipeline Demo

A demonstration Node.js application showcasing CI/CD pipeline integration with both **GitHub Actions** and **Azure DevOps Pipelines**.

## 🚀 Overview

This project is a simple Express.js web server designed to demonstrate automated build and test workflows across multiple CI/CD platforms. It serves as a template for setting up continuous integration in your Node.js projects.

## 📋 Features

- **Express.js Server**: Lightweight web server running on port 3000
- **GitHub Actions**: Automated CI workflow testing across Node.js versions 18.x, 20.x, and 22.x
- **Azure Pipelines**: Pre-configured Azure DevOps pipeline integration
- **Jest Testing**: Test framework setup and ready for expansion
- **Multi-version Testing**: Ensures compatibility across multiple Node.js versions

## 🛠️ Getting Started

### Prerequisites

- Node.js (18.x, 20.x, or 22.x recommended)
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/joshjones-jp/pipeline.git
cd pipeline

# Install dependencies
npm install
```

### Running Locally

```bash
# Start the server
npm start

# The app will be available at http://localhost:3000
```

You should see the message: **"Hello from GitHub Actions + Azure! 🚀"**

## 🧪 Testing

```bash
# Run tests
npm test

# Run linting (when configured)
npm run lint
```

## 🔄 CI/CD Pipelines

### GitHub Actions

The project includes a GitHub Actions workflow (`.github/workflows/node-ci.yml`) that:
- Triggers on pushes and pull requests to the `main` branch
- Tests across Node.js versions 18.x, 20.x, and 22.x
- Runs linting and tests automatically

### Azure DevOps Pipelines

Azure Pipelines configuration files are included:
- `azure-pipelines.yml`
- `azure-pipelines-1.yml`
- `AZDO.yml`

These pipelines:
- Use Ubuntu-latest as the build environment
- Install Node.js 20.x
- Run `npm install` and `npm run build`

## 📂 Project Structure

```
pipeline/
├── .github/
│   └── workflows/
│       └── node-ci.yml          # GitHub Actions workflow
├── test/
│   └── basic.test.js            # Jest test file
├── .gitignore
├── AZDO.yml                     # Azure DevOps pipeline
├── azure-pipelines.yml          # Azure DevOps pipeline
├── azure-pipelines-1.yml        # Azure DevOps pipeline
├── package.json                 # Project dependencies and scripts
├── server.js                    # Express.js server
└── README.md                    # This file
```

## 🚧 Roadmap / To-Do

- [ ] Expand test coverage for server endpoints
- [ ] Add ESLint configuration for code linting
- [ ] Implement build script or update Azure pipelines
- [ ] Add more robust API endpoints
- [ ] Add deployment configurations
- [ ] Include code coverage reporting

## 🤝 Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

## 📄 License

This project is open source and available for educational and demonstration purposes.

## 👤 Author

**joshjones-jp**

---

⭐ If you find this project helpful, consider giving it a star on GitHub!