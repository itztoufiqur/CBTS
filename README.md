# College Bus Tracking and Notification System

This project provides a system to track the location of college buses and send notifications to students when the bus reaches their location. The project also includes a chat functionality allowing students to communicate with the bus driver. The project is divided into three main components:

![image](https://github.com/user-attachments/assets/50b0b99d-409b-4a03-b5d1-66871bbb4c42)


1. **Solidity Smart Contract**: Manages user roles (Student/Driver).
2. **Backend Server**: Handles location tracking, notifications, and chat functionality.
3. **Frontend**: A user interface for both students and drivers to interact with the system.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Solidity Contract](#solidity-contract)
- [Backend Setup](#backend-setup)
- [Frontend Setup](#frontend-setup)
- [Contributing](#contributing)
- [Developer Contact](#developer-contact)
- [License](#license)

## Features

- **User Role Management**: Users can register as either a student or a bus driver.
- **Real-time Location Tracking**: Track the real-time location of buses.
- **Notifications**: Notify students when the bus is near their location.
- **Chat Functionality**: Students can communicate with the bus driver.

## Installation

### Prerequisites

- Node.js (v14.x or higher)
- Truffle (for deploying Solidity contracts)
- Ganache (for local Ethereum blockchain)
- A web3 provider (like MetaMask) for interacting with the smart contract
- Python (if using a Python backend) or any other backend framework like Express.js

### Clone the Repository

```bash
git clone https://github.com/your-username/college-bus-tracking.git
cd college-bus-tracking
```

### Install Dependencies

Navigate to each directory (`backend`, `frontend`, `smart-contracts`) and run the following command to install the necessary packages:

```bash
npm install
```

## Usage

### 1. Deploy the Smart Contract

Navigate to the `smart-contracts` directory and deploy the contract to your local blockchain:

```bash
truffle migrate --network development
```

### 2. Start the Backend Server

Navigate to the `backend` directory and start the server:

```bash
npm start
```

### 3. Run the Frontend

Navigate to the `frontend` directory and start the application:

```bash
npm start
```

## Solidity Contract

The Solidity contract is located in the `smart-contracts/contracts/BusTracking.sol` file. It manages the registration of users as either students or drivers.
## Contract add : 0xcD6a42782d230D7c13A74ddec5dD140e55499Df9

### Contract Functions

- `registerUser(string memory _name, UserType _userType)`: Register a user as a student or driver.
- `getUser(address _userAddress)`: Retrieve user details by their address.

## Backend Setup

The backend server handles location tracking, notifications, and chat functionalities. It communicates with the smart contract to verify user roles.

### Backend Structure

- **Location Tracking**: Handles GPS coordinates and calculates proximity to the student's location.
- **Notifications**: Sends notifications to students using services like Firebase or Twilio.
- **Chat**: Enables real-time communication between students and drivers using WebSocket.

### Running the Backend

```bash
npm start
```

## Frontend Setup

The frontend is a web or mobile application that allows users to interact with the system. It interfaces with both the backend and the smart contract.

### Frontend Structure

- **Student Interface**: Allows students to see the bus location, receive notifications, and chat with the driver.
- **Driver Interface**: Allows drivers to update their location and communicate with students.

### Running the Frontend

```bash
npm start
```

## Contributing

Contributions are welcome! Please follow the steps below:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -am 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Create a new Pull Request.

## Developer Contact

For any questions or issues related to this project, please contact the developer:

- **Name:** [Toufiqur Rahman]
- **Email:** [its.toufiqur@gmail.com]
- **LinkedIn:** [[Your LinkedIn Profile](https://www.linkedin.com/in/toufiqur-rahman-499549311/)
- **GitHub:** [Your GitHub Profile](https://github.com/itztoufiqur)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```
