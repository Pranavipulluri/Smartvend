SmartVend: Sanitary Pad Vending Machine Web App

SmartVend is a web-based interface for a smart sanitary pad vending machine. This application allows users to select and purchase sanitary pads through a simple and seamless interface, while also providing an admin portal to manage stock and monitor low-stock alerts.

Features

User Side

Sanitary Pad Selection: Users can choose the number of pads (up to a maximum of 5 at a time).

Real-Time Stock Display: Shows available pads in the machine.

Payment Integration: Razorpay gateway integration for smooth and secure transactions.

Dispensing Simulation: Visual feedback showing the dispensing process.

Low Stock Alert: Notifies admin when stock falls below a certain threshold.

Admin Side

Authentication: Admin login with a password.

Stock Management: Add or set available pad count.

Low Stock Notification: Backend alert when pads are running low.

Tech Stack

Frontend: React.js, Tailwind CSS

Backend: Node.js, Express

Database: Firebase (for future stock management)

Payment Gateway: Razorpay

Setup and Installation

Clone the repository:

git clone https://github.com/your-repo-url/smartvend.git
cd smartvend

Install dependencies:

npm install

Run the development server:

npm start

Backend Setup: (Ensure your backend server is running)

cd backend
npm install
node server.js

Environment Variables

Create a .env file in the root directory and add:

REACT_APP_RAZORPAY_KEY=your_razorpay_public_key
BACKEND_URL=http://localhost:5000

API Endpoints

Create Order: POST /create-order

Verify Payment: POST /verify-payment

Low Stock Alert: POST /low-stock-alert

Future Enhancements

Firebase integration for real-time stock updates.

More secure admin authentication.

Improved UI/UX.

Enhanced error handling.

License

This project is licensed under the MIT License.

Contributors

Goutham - Team leader
Pranavi - Developer
Sarvani - Developer

SmartVend: Making hygiene accessible, one pad at a time.
