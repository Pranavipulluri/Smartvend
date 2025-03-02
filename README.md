# SmartVend: Digital Sanitary Pad Vending System

## Overview

SmartVend is a modern solution for digitalizing sanitary pad vending machines, ensuring seamless access to menstrual hygiene products. By integrating digital payment methods, inventory tracking, and real-time monitoring, SmartVend enhances both user convenience and operational efficiency.

The system consists of a web interface for users to purchase products and an admin panel for inventory management, making hygiene products more accessible while ensuring efficient maintenance and restocking.

---

## Features

- **User-Friendly Interface**: Simple UI for selecting quantity and completing purchases
- **Digital Payments**: Integrated with Razorpay for secure UPI transactions
- **Real-Time Inventory Tracking**: Automatic monitoring of available products
- **Low Stock Alerts**: Automated notifications when inventory reaches threshold levels
- **Admin Dashboard**: For restocking and managing machines
- **Machine Identification**: Each machine has a unique ID for location tracking
- **Mobile Responsive**: Accessible on any device

---

## Tech Stack

- **Frontend**: React.js, TailwindCSS
- **Payment Gateway**: Razorpay
- **Backend**: Node.js/Express.js (implied from API endpoints)
- **Authentication**: Admin password protection

---

## Installation

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- Razorpay account for payment processing

### Setup Steps

1. Clone the repository:
```bash
git clone https://github.com/your-username/smartvend.git
cd smartvend
```

2. Install dependencies:
```bash
npm install
# or
yarn install
```

3. Configure environment variables:
Create a `.env` file in the root directory with the following variables:
```
REACT_APP_RAZORPAY_KEY=your_razorpay_key
REACT_APP_BACKEND_URL=http://localhost:5000
```

4. Start the development server:
```bash
npm start
# or
yarn start
```

5. The application should now be running at `http://localhost:3000`

---

## Backend Setup (Required)

The frontend expects a backend server running at `http://localhost:5000` with the following endpoints:

- `POST /create-order`: Creates a new payment order
- `POST /verify-payment`: Verifies payment completion
- `POST /low-stock-alert`: Sends notifications when stock is low

Refer to the backend repository for setup instructions.

---

## Usage

### User Flow

1. User selects the number of pads required (1-5)
2. System displays the total cost
3. User clicks "Proceed to Payment" button
4. Razorpay payment gateway opens
5. After successful payment, the machine dispenses the selected number of pads

### Admin Flow

1. Click the "Admin" button in the top-right corner
2. Enter the admin password (default: "admin123")
3. Choose to either add to existing inventory or set a new total
4. Enter the quantity
5. Click "Add Inventory" or "Update Inventory" to save changes

---

## Security

- Admin access is protected by password authentication
- Payments are processed securely through Razorpay
- Machine IDs are unique to prevent tampering

---

## Deployment

To build the application for production:

```bash
npm run build
# or
yarn build
```

The build artifacts will be stored in the `build/` directory, ready to be deployed to a web server.

---

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## Future Enhancements

- **Mobile App**: Development of a companion app to display machine locations and available stock
- **Analytics Dashboard**: For tracking usage patterns and optimizing inventory management
- **Multiple Product Support**: Expanding to support different types of hygiene products
- **QR Code Integration**: For faster access to specific machines
- **User Accounts**: Optional accounts for frequent users with purchase history

---

## License

This project is licensed under the MIT License - see the LICENSE file for details.

---

## Acknowledgments

- Razorpay for payment gateway integration
- TailwindCSS for the UI components
- React.js community for the frontend framework

---

## Contact

Project Link: [https://github.com/your-username/smartvend](https://github.com/your-username/smartvend)
