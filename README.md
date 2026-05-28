🍽️ Homely Meals

A modern food delivery platform connecting home cooks with customers.



📖 About The Project

Homely Meals is a comprehensive food delivery platform that empowers home cooks to turn their culinary skills into a business. Customers can discover authentic homemade meals, while cooks manage their menu and orders through an intuitive dashboard. Administrators oversee the entire ecosystem to ensure quality and safety.

✨ Key Features

👥 For Customers

🔍 Browse meals from verified home cooks

🛒 Easy ordering with secure payment

📍 Real-time order tracking with maps

⭐ Rate and review meals

💬 Chat directly with cooks

📊 View order history and analytics

👨‍🍳 For Cooks

📝 Create and manage meal menus

📦 Handle orders with status updates

💰 Track sales and revenue

📈 View detailed analytics dashboard

📄 Upload verification documents

🔔 Real-time order notifications

📱 PWA support for mobile experience

🛡️ For Admins

✅ Verify and approve new cooks

👤 Manage customers and cooks

📋 Monitor all orders

🚨 Handle complaints and disputes

⚙️ Configure delivery charges

📊 System-wide analytics

🛠️ Built With

Frontend

⚛️ React 19 - UI framework

⚡ Vite - Build tool

🎨 Tailwind CSS - Styling

🧭 React Router - Navigation

📡 Axios - HTTP client

🔌 Socket.IO - Real-time communication

🗺️ Leaflet - Interactive maps

📊 Recharts - Data visualization

💳 Stripe - Payment processing

Backend

🟢 Node.js - Runtime environment

🚂 Express.js - Web framework

🍃 MongoDB - Database

🔐 JWT - Authentication

💳 Stripe - Payment gateway

📧 Nodemailer - Email service

🔔 Web Push - Push notifications

🤖 Groq AI - AI integration

📁 Project Structure

HomelyMeals/
│
├── 📱 admin-ui/     # Admin dashboard
├── 👨‍🍳 cook/       # Cook application (PWA)
├── 👥 customer/     # Customer application
└── 🖥️ server/       # Backend API

🚀 Getting Started

📋 Prerequisites

Before you begin, ensure you have the following installed:

📦 Node.js (v16 or higher) - https://nodejs.org/

🍃 MongoDB - https://www.mongodb.com/try/download/community

☁️ MongoDB Atlas (Optional) - https://www.mongodb.com/cloud/atlas

💳 Stripe Account - https://stripe.com/

☁️ Cloudinary Account - https://cloudinary.com/

📥 Installation

1️⃣ Clone the Repository

git clone https://github.com/yourusername/homely-meals.git
cd homely-meals

2️⃣ Install Server Dependencies

cd server
npm install

3️⃣ Install Admin UI Dependencies

cd ../admin-ui
npm install

4️⃣ Install Cook App Dependencies

cd ../cook
npm install

5️⃣ Install Customer App Dependencies

cd ../customer
npm install

⚙️ Configuration

🖥️ Server Environment Variables

Create a .env file inside the server folder:

# 🌐 Server
PORT=5000
NODE_ENV=development

# 🗄️ Database
MONGODB_URI=mongodb://localhost:27017/homely-meals

# 🔐 Authentication
JWT_SECRET=your_super_secret_jwt_key_here
JWT_EXPIRE=7d

# 💳 Stripe
STRIPE_SECRET_KEY=sk_test_your_stripe_secret_key
STRIPE_PUBLISHABLE_KEY=pk_test_your_stripe_publishable_key

# 📧 Email
RESEND_API_KEY=your_resend_api_key
FROM_EMAIL=noreply@yourdomain.com

# ☁️ Cloudinary
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

# 🔔 Push Notifications
VAPID_PUBLIC_KEY=your_vapid_public_key
VAPID_PRIVATE_KEY=your_vapid_private_key

# 🤖 AI
GROQ_API_KEY=your_groq_api_key

🌐 Frontend Environment Variables

Create .env files inside admin-ui, cook, and customer folders:

# 🔌 API
VITE_API_URL=http://localhost:5000/api
VITE_SOCKET_URL=http://localhost:5000

# 💳 Stripe
VITE_STRIPE_PUBLISHABLE_KEY=pk_test_your_stripe_publishable_key

# ☁️ Cloudinary
VITE_CLOUDINARY_CLOUD_NAME=your_cloud_name
VITE_CLOUDINARY_UPLOAD_PRESET=your_upload_preset

# 🔔 Push Notifications (Cook App Only)
VITE_VAPID_PUBLIC_KEY=your_vapid_public_key

🏃‍♂️ Running the Application

🔧 Development Mode

Open 4 separate terminals and run:

🖥️ Terminal 1 - Backend Server

cd server
npm run dev

✅ Server running at: http://localhost:5000

🛡️ Terminal 2 - Admin Dashboard

cd admin-ui
npm run dev

✅ Admin UI running at: http://localhost:5173

👨‍🍳 Terminal 3 - Cook App

cd cook
npm run dev

✅ Cook app running at: http://localhost:5174

👥 Terminal 4 - Customer App

cd customer
npm run dev

✅ Customer app running at: http://localhost:5175

🚀 Production Build

Build All Frontend Apps

cd admin-ui && npm run build

cd ../cook && npm run build

cd ../customer && npm run build

Start Production Server

cd ../server
npm start

📚 API Endpoints

🔐 Authentication

POST   /api/auth/register
POST   /api/auth/login
POST   /api/auth/logout
POST   /api/auth/verify-otp

👨‍🍳 Cooks

GET    /api/cooks
GET    /api/cooks/:id
PUT    /api/cooks/:id
POST   /api/cooks/documents

👥 Customers

GET    /api/customers
GET    /api/customers/:id
PUT    /api/customers/:id

🍽️ Meals

GET    /api/meals
POST   /api/meals
PUT    /api/meals/:id
DELETE /api/meals/:id

📦 Orders

GET    /api/orders
POST   /api/orders
GET    /api/orders/:id
PUT    /api/orders/:id/status

💳 Payments

POST   /api/payments/create-intent
POST   /api/payments/webhook

📋 Subscriptions

GET    /api/subscriptions
POST   /api/subscriptions
PUT    /api/subscriptions/:id
DELETE /api/subscriptions/:id

🌐 Deployment

Backend Deployment Options

🚂 Railway

☁️ Render

🟣 Heroku

🌊 DigitalOcean

☁️ AWS EC2

Frontend Deployment Options

▲ Vercel ⭐ Recommended

🌐 Netlify

🔥 Firebase Hosting

Database

🍃 MongoDB Atlas ⭐ Recommended

🖥️ Self-hosted MongoDB

🤝 Contributing

Contributions are what make the open-source community amazing. Any contributions you make are greatly appreciated.

# Fork the Project

# Create your Feature Branch
git checkout -b feature/AmazingFeature

# Commit your Changes
git commit -m "Add some AmazingFeature"

# Push to the Branch
git push origin feature/AmazingFeature

Then open a Pull Request 🚀

📝 License

Distributed under the ISC License. See the LICENSE file for more information.

👨‍💻 Author

Your Name

GitHub: @yourusername

Email: your.email@example.com

🙏 Acknowledgments

React - Amazing UI library

Vite - Lightning fast build tool

MongoDB - Flexible database

Stripe - Secure payments

Tailwind CSS - Utility-first CSS

📞 Support

Need help?

📧 Email: support@homelymeals.com

💬 Open an issue on GitHub

📖 Check the documentation

⭐ Star this repository if you found it helpful!

Made with ❤️ by the HomelyMeals Team
