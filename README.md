# IntegerSet API

## Overview

The `IntegerSet API` is a simple RESTful web service implemented using Python's Flask framework. The service provides an API to manage a set of integers, allowing clients to add, check, and remove integers from the set.

## Features

- **Add an Integer**: Add a unique integer to the set.
- **Check Integer Existence**: Verify if a specific integer is in the set.
- **Remove an Integer**: Remove a specific integer from the set.

## Installation

### Prerequisites

- Python 3.x
- Flask

### Steps

1. **Clone the repository:**

    ```sh
    git clone https://github.com/your_username/integer-set-api.git
    cd integer-set-api
    ```

2. **Create a virtual environment (optional but recommended):**

    ```sh
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the required dependencies:**

    ```sh
    pip install -r requirements.txt
    ```

## Usage

1. **Run the Flask application:**

    ```sh
    python app.py
    ```

   The application will start and be accessible at `http://0.0.0.0:8080`.

2. **API Endpoints**

    - **Add an Integer:**

      ```http
      POST /add
      ```

      **Request Body:**

      ```json
      {
          "item": 1
      }
      ```

      **Response:**

      - 201: Integer added successfully
      - 400: Error message if the integer already exists or if the input is invalid

    - **Check Integer Existence:**

      ```http
      GET /has?itemId=1
      ```

      **Response:**

      - 200: Integer exists in the set
      - 404: Integer does not exist
      - 400: Error message if the `itemId` is invalid

    - **Remove an Integer:**

      ```http
      POST /remove
      ```

      **Request Body:**

      ```json
      {
          "itemId": 1
      }
      ```
      **Response:**

      - 200: Integer removed successfully
      - 404: Integer not found
      - 400: Error message if the `itemId` is invalid
     
# Cloud Formation
![image](https://github.com/user-attachments/assets/941fb947-c198-46d4-b143-446d62b11451)


# EC2 Instance
![image](https://github.com/user-attachments/assets/22b02872-ce3d-445e-b9e6-d4d1004fc6ed)


# Remote Server on VS code
![image](https://github.com/user-attachments/assets/92804771-e805-47ae-ba95-473a60acb2ad)


