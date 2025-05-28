# API Auto Tester Pro 🚀

A powerful, user-friendly web-based tool for automated API testing. Upload your API configuration files and get comprehensive test results with beautiful visualizations.

![API Auto Tester Pro](https://img.shields.io/badge/API-Auto%20Tester%20Pro-blue?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

## ✨ Features

- **📁 Drag & Drop File Upload** - Simply drag your JSON configuration file into the interface
- **🔐 Bearer Token Authentication** - Built-in support for API authentication with secure token storage
- **⚡ Batch API Testing** - Test multiple endpoints simultaneously with progress tracking
- **📊 Real-time Results** - Live status updates and detailed response analysis
- **🎨 Beautiful UI** - Clean, responsive interface built with TailwindCSS
- **📋 Export Results** - Copy all test results to clipboard for documentation
- **🔍 Response Viewer** - JSON syntax highlighting and collapsible response sections
- **⏱️ Performance Metrics** - Response time and payload size tracking
- **🚨 Error Handling** - Comprehensive error reporting with detailed debugging information

## 🎯 Use Cases

- **API Development Testing** - Quickly validate your API endpoints during development
- **Integration Testing** - Test multiple API endpoints in sequence
- **API Documentation** - Generate test results for API documentation
- **Quality Assurance** - Automated testing for QA teams
- **Learning & Development** - Perfect for learning API testing concepts

## 🚀 Quick Start

### 1. Setup
Simply open the `index.html` file in any modern web browser. No installation or server setup required!

### 2. Configure Authentication (Optional)
If your APIs require authentication:
1. Enter your Bearer token in the Authentication section
2. Click "Save" to store it securely in your browser
3. The token will be automatically included in all API requests

### 3. Prepare Your API Configuration
Create a JSON file with your API endpoints. See the [Configuration Format](#-configuration-format) section below.

### 4. Upload & Test
1. Drag and drop your JSON file into the upload area
2. Review the loaded endpoints
3. Click "Run Tests" to start testing
4. Monitor progress and view results in real-time

## 📋 Configuration Format

Your JSON file should contain an array of API endpoint objects. Each object represents a single API request.

### Required Fields
- `endpoint` (string): The full URL of the API endpoint
- `method` (string): HTTP method (GET, POST, PUT, DELETE, PATCH)

### Optional Fields
- `data` (object): Request payload for POST, PUT, PATCH requests
- `headers` (object): Custom headers for the request
- `params` (object): URL query parameters

### Example Configuration Files

#### Basic GET Requests
```json
[
    {
        "endpoint": "https://api.example.com/users",
        "method": "GET"
    },
    {
        "endpoint": "https://api.example.com/users/123",
        "method": "GET"
    }
]