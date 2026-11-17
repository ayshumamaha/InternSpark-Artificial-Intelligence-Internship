# Model Deployment Using Flask and Docker

## 1. Project Overview

The Model Deployment Project is a Python application that demonstrates how a trained machine learning model can be deployed as a web API. It uses the Iris dataset to train a Random Forest classification model and provides prediction functionality through a Flask application.

The application exposes API endpoints that allow users to check the service status and submit input features for predictions. It accepts data in JSON format and returns the predicted Iris flower class along with prediction probabilities.

The project also demonstrates containerization using Docker by providing a Dockerfile and requirements file to package the application and its dependencies.

## 2. Objectives

- Deploy a machine learning model using Flask.
- Develop API endpoints for model inference.
- Accept input data through JSON requests.
- Return predictions in JSON format.
- Understand API testing and response handling.
- Containerize the application using Docker.
- Learn how to run a deployed model locally and inside a Docker container.

## 3. Tools and Technologies Used

- **Programming Language:** Python
- **Web Framework:** Flask
- **Machine Learning Library:** Scikit-learn
- **Additional Libraries:** NumPy
- **Containerization Tool:** Docker
- **Dataset:** Iris Dataset
- **Concepts:** REST API, model inference, JSON, HTTP requests, containerization

## 4. Features Implemented

- Trains a Random Forest classifier using the Iris dataset.
- Creates a Flask web application.
- Implements a `/health` endpoint to check API availability.
- Implements a `/predict` endpoint for machine learning predictions.
- Accepts four numerical input features in JSON format.
- Validates incoming prediction data.
- Returns the predicted flower class.
- Provides prediction probabilities.
- Handles invalid inputs and request errors.
- Generates a Dockerfile and requirements file.
- Supports local execution and Docker-based deployment.

## 5. How to Run the Program

1. Install Python on your system.
2. Install the required libraries:

```bash
pip install flask numpy scikit-learn
```

3. Save the program as `model_deployment.py`.
4. Open a terminal and navigate to the project folder.
5. Run the application:

```bash
python model_deployment.py
```

6. The Flask application starts on port 5000.
7. Test the health endpoint using:

```bash
curl http://localhost:5000/health
```

8. Test the prediction endpoint using:

```bash
curl -X POST http://localhost:5000/predict -H "Content-Type: application/json" -d "{\"features\":[5.1,3.5,1.4,0.2]}"
```

### Running with Docker

After running the Python program once to generate the Dockerfile and requirements file, build the Docker image:

```bash
docker build -t ml-api .
```

Run the container:

```bash
docker run -p 5000:5000 ml-api
```

The API can then be accessed locally through port 5000.

## 6. Expected Output

The application starts a Flask server and provides responses through its API endpoints.

The health endpoint returns a response indicating that the API is running. The prediction endpoint accepts flower measurements and returns the predicted Iris species and its associated probabilities in JSON format.

The application can also be packaged and executed inside a Docker container.

## 7. Learning Outcomes

- Understanding machine learning model deployment.
- Developing REST APIs using Flask.
- Working with JSON request and response formats.
- Implementing model inference endpoints.
- Validating API inputs.
- Testing API functionality using curl.
- Understanding Dockerfiles and containerization.
- Running machine learning applications in containers.

## Author

M. Ayshwarya
