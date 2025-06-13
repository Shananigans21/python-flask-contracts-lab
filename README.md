# Flask Contracts API

This project is a simple Flask web application that demonstrates building dynamic routes and handling HTTP status codes. It includes routes to retrieve contract and customer information.

---

## Routes

###  `GET /contracts/<int:id>`
- **Description**: Fetches contract information by contract ID.
- **Response**:
  - `200 OK`: If the contract is found, returns the contract details as JSON.
  - `404 Not Found`: If no contract is found for the given ID.

**Example**:

GET /contracts/1
Response: {
"contract": {
"id": 1,
"contract_information": "This contract is for John and building a shed"
}
}


---

###  `GET /customers/<customer_name>`
- **Description**: Checks if a customer exists in the system.
- **Response**:
  - `204 No Content`: If the customer is found.
  - `404 Not Found`: If the customer is not found.

**Example**:
GET /customers/bob
Response: [Blank page with 204 status]


---

##  Getting Started

### Prerequisites
- Python 3 installed
- Flask installed

### Run the app:
```bash
export FLASK_APP=app.py
python3 app.py
