# Dealer Evaluation Frontend

This project contains the frontend for the dealer evaluation system, built using Flask and React.

## Getting Started

### Prerequisites

- Python 3.13
- Node.js (for React frontend)
- Docker (optional, for containerization)

### Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Application

```bash
python app.py
```

## Usage
To build and run using IBM Cloud CE:
```bash
ibmcloud ce application create --name frontend --image us.icr.io/${SN_ICR_NAMESPACE}/prodlist --registry-secret icr-secret --port 5001 --build-source .
```

Other Command
```bash
# Get Deployed Instances
ibmcloud ce app get --name frontend -q
# Update set min. Instances
ibmcloud ce app update --name frontend --min 2
# To delete the application
ibmcloud ce application delete --name frontend
```

## Project Structure

```
dealer_evaluation_frontend/
├── app.py
├── Dockerfile
└── html/
    └── index.html
```