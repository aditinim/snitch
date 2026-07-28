# Snitch

Snitch is a full-stack e-commerce marketplace built using the MERN stack. It enables buyers to discover and purchase products while providing sellers with a dedicated dashboard to manage products, inventory, and sales. The application implements secure authentication, product variants, cloud-based image uploads, shopping cart management, and online payments through Razorpay.

## Features

### Authentication

* Secure user registration and login
* JWT-based authentication
* Google OAuth login
* Protected routes
* Role-based access control (Buyer & Seller)

### Buyer Features

* Browse products
* View product details
* Select product variants
* Add products to cart
* Secure checkout
* Online payments using Razorpay

### Seller Features

* Seller dashboard
* Add and manage products
* Upload multiple product images
* Create and manage product variants
* Inventory management

### Product Management

* Multiple image support
* Variant-based products (Size, Colour, etc.)
* Stock management
* Dynamic pricing

### Payments

* Razorpay payment gateway integration
* Secure payment verification
* Order confirmation workflow

### Image Upload

* Cloud image storage using ImageKit
* Optimized image delivery

---

## Tech Stack

### Frontend

* React.js
* Vite
* Tailwind CSS
* Redux Toolkit
* React Router
* Axios

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose

### Authentication

* JWT
* Google OAuth
* Cookies

### Third-Party Services

* ImageKit
* Razorpay

---

## Project Structure

```text
Snitch
│
├── frontend
│   ├── src
│   │   ├── components
│   │   ├── features
│   │   ├── hooks
│   │   ├── pages
│   │   ├── services
│   │   ├── store
│   │   └── utils
│   └── public
│
├── backend
│   ├── config
│   ├── controllers
│   ├── dao
│   ├── middleware
│   ├── models
│   ├── routes
│   ├── services
│   └── validators
│
└── README.md
```

---

## System Architecture

```text
                 React Frontend
                        │
                  Axios API Calls
                        │
                Express Backend
                        │
        Authentication Middleware
                        │
                  Controllers
                        │
                 Services / DAO
                        │
                    MongoDB
```

---

## Application Workflow

### Buyer Workflow

```text
Browse Products
        │
        ▼
View Product Details
        │
        ▼
Select Variant
        │
        ▼
Add to Cart
        │
        ▼
Checkout
        │
        ▼
Razorpay Payment
        │
        ▼
Order Confirmation
```

### Seller Workflow

```text
Seller Login
      │
      ▼
Seller Dashboard
      │
      ▼
Create Product
      │
      ▼
Upload Product Images
      │
      ▼
Create Product Variants
      │
      ▼
Publish Product
```

### Authentication Flow

```text
Register / Login
        │
        ▼
Credentials Validation
        │
        ▼
JWT Generation
        │
        ▼
Cookie Storage
        │
        ▼
Protected API Access
```

### Payment Workflow

```text
Checkout
    │
    ▼
Create Razorpay Order
    │
    ▼
Complete Payment
    │
    ▼
Payment Verification
    │
    ▼
Order Confirmation
```

---

## Installation

### Prerequisites

* Node.js
* MongoDB
* npm

### Clone the Repository

```bash
git clone https://github.com/your-username/snitch.git

cd snitch
```

---

## Backend Setup

```bash
cd backend

npm install
```

Create a `.env` file inside the **backend** directory.

```env
PORT=

MONGO_URI=

JWT_SECRET=

CLIENT_URL=

GOOGLE_CLIENT_ID=
GOOGLE_CLIENT_SECRET=

IMAGEKIT_PUBLIC_KEY=
IMAGEKIT_PRIVATE_KEY=
IMAGEKIT_URL_ENDPOINT=

RAZORPAY_KEY_ID=
RAZORPAY_KEY_SECRET=
```

Start the backend server.

```bash
npm run dev
```

---

## Frontend Setup

```bash
cd frontend

npm install
```

Create a `.env` file inside the **frontend** directory.

```env
VITE_API_URL=

VITE_RAZORPAY_KEY=
```

Start the frontend server.

```bash
npm run dev
```

---

## Future Enhancements

* Order history
* Wishlist
* Product reviews and ratings
* Search and advanced filtering
* Coupons and discounts
* Admin dashboard
* Seller analytics
* Shipment tracking
* Email notifications
* Recommendation system

---

## Learning Outcomes

This project provided hands-on experience with:

* Full-stack web development
* REST API development
* JWT authentication
* Google OAuth integration
* MongoDB data modelling
* Cloud image management
* Payment gateway integration
* Redux state management
* Feature-based React architecture
* Layered backend architecture
* Building scalable web applications

---

## Contributing

Contributions are welcome. Feel free to fork the repository, create a new branch, and submit a pull request.

```bash
git checkout -b feature/new-feature
git commit -m "Add new feature"
git push origin feature/new-feature
```

---

## License

This project is licensed under the MIT License.

---

## Author

**Aditi Nim**

If you found this project useful, consider giving it a ⭐ on GitHub.
