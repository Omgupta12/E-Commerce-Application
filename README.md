# E-Commerce-Application

This is a full-stack e-commerce platform built with the MERN stack (MongoDB, Express.js, React.js, and Node.js). It allows users to browse products, add them to a shopping cart, make purchases, and manage their accounts.

## Features
- User authentication (JWT-based)
- Product listing and details page
- Shopping cart functionality
- Checkout and payment integration (Stripe & Cash Pickup)
- Order tracking and user dashboard
- Admin dashboard for product management
- Responsive UI with React.js and Tailwind CSS

## Tech Stack
- **Frontend**: React.js, Tailwind CSS
- **Backend**: Node.js, Express.js, MongoDB
- **Database**: MongoDB with Mongoose ORM
- **Authentication**: JWT (JSON Web Tokens)
- **Payment**: Stripe, Cash Pickup

---

## Installation and Setup

### Prerequisites
Ensure you have the following installed on your system:
- [Node.js](https://nodejs.org/) (v14+ recommended)
- [MongoDB](https://www.mongodb.com/try/download/community) (local or cloud-based MongoDB Atlas)
- [Git](https://git-scm.com/)

### Clone the Repository
```sh
git clone https://github.com/Omgupta12/E-Commerce-Application.git
cd E-Commerce-Application
```

### Backend Setup
1. Navigate to the backend directory:
   ```sh
   cd backend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Create a `.env` file in the `backend` directory and add the following:
   ```env
   PORT=4000
   MONGODB_URI='your_mongodb_connection_string'
   JWT_SECRET='your_jwt_secret_key'
   STRIPE_SECRET_KEY='your_stripe_secret_key'
   CLOUDINARY_API_KEY='your_cloudinary_api_key'
   CLOUDINARY_SECRET_KEY='your_cloudinary_secret_key'
   CLOUDINARY_NAME='your_cloudinary_name'
   ```
4. Run the backend server:
   ```sh
   npm start
   ```

### Frontend Setup
1. Navigate to the frontend directory:
   ```sh
   cd frontend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Create a `.env` file in the `frontend` directory and add the following:
   ```env
   VITE_API_URL=http://localhost:4000
   ```
4. Start the frontend server:
   ```sh
   npm run dev
   ```
   
   ### Admin Panel Setup
1. Navigate to the admin directory:
   ```sh
   cd admin
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Create a `.env` file in the `admin` directory and add the following:
   ```env
   VITE_API_URL=http://localhost:4000
   ```
4. Start the admin panel server:
   ```sh
   npm run dev
   ```

The application should now be running on:
- Frontend: `http://localhost:5173`
- Backend: `http://localhost:4000`
- Admin Panel: `http://localhost:5174`

---

## Deployment

### Deploy Backend, Frontend, and Admin to Vercel
1. Create an account on [Vercel](https://vercel.com/).
2. Connect your GitHub repository.
3. Deploy backend by selecting the `backend` folder.
4. Deploy frontend by selecting the `frontend` folder.
5. Deploy admin panel by selecting the `admin` folder.
6. Set up environment variables in each project as per the `.env` files.
7. Deploy the projects.

---

## API Endpoints
### Authentication
- `POST /api/user/register` - Register a new user
- `POST /api/user/login` - Login user
- `POST /api/user/admin` - Login admin

### Products
- `GET /api/product/list` - Get all products
- `GET /api/product/single` - Get product details
- `POST /api/product/add` - Add new product (Admin only)
- `DELETE /api/product/remove` - Remove product (Admin only)

### Cart & Orders
- `POST /api/cart/add` - Add item to cart
- `GET /api/cart/get` - Get cart items
- `PUT /api/cart/update` - Update cart item
- `POST /api/order/userorders` - Place order
- `GET /api/order/list` - Get All Order
---
## Screenshot's 
### 1. Home Page
![image](https://github.com/user-attachments/assets/588cf278-6a15-43f1-906d-8b9a7a351d65)
![image](https://github.com/user-attachments/assets/032dccb4-f91d-4c90-bd9f-ba98f03cb004)
### 2. Product List Page
![image](https://github.com/user-attachments/assets/eedfa253-c78b-41a4-bbfe-19536c65721a)
### 3. Product Detail Page
![image](https://github.com/user-attachments/assets/7927c91a-c740-42f2-a1e9-7ea2342cad5f)
### 4. Cart Page
![image](https://github.com/user-attachments/assets/10fd73ff-293b-41d8-b706-05282c72f102)
### 5. Place Order Page
![image](https://github.com/user-attachments/assets/85918504-675a-40cb-82d0-b9aa3962668f)
### 6. User Order Page
![image](https://github.com/user-attachments/assets/5b718c77-0f9f-42bb-96c0-c0c08e7aa4cf)
### 7. Login Page
![image](https://github.com/user-attachments/assets/36aeae4e-64ad-4fd4-a656-b6c50c0f4cee)
### 8. Admin List Page
![image](https://github.com/user-attachments/assets/12ba71b5-da9b-4b32-8252-f7552be33470)

## Contributing
Contributions are welcome! Feel free to fork the repository and submit a pull request.

## License
This project is licensed under the MIT License.
