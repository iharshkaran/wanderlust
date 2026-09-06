# 🧭 WanderLust

**WanderLust** is a full-stack holiday rental web application designed to make discovering and sharing unique stays simple and interactive.

Users can explore available properties, view their locations on an interactive map, create and manage their own listings, upload property images, and share reviews and ratings with the community.

---

## 🌟 Highlights

* 🏡 Explore and discover holiday stays
* 🔐 Secure user authentication and authorization
* ➕ Create and publish property listings
* ✏️ Edit and manage your own listings
* 🗑️ Delete listings when needed
* ☁️ Upload and manage property images using Cloudinary
* 🗺️ View property locations using interactive maps
* 🏷️ Browse properties using category filters
* ⭐ Add ratings and reviews to listings
* 💰 Dynamic price calculation with tax support
* 📱 Responsive design for desktop and mobile devices

---

## 🛠️ Tech Stack

### Frontend

* HTML5
* CSS3
* JavaScript
* Bootstrap 5
* EJS
* EJS-Mate

### Backend

* Node.js
* Express.js

### Database

* MongoDB
* Mongoose

### Authentication

* Passport.js
* Passport-Local
* Express Session
* Connect-Mongo

### Image & Map Services

* Cloudinary
* Multer
* Leaflet.js
* OpenStreetMap
* Nominatim Geocoding API

---

## 📂 Project Structure

```text
WanderLust/
│
├── controllers/        # Application controllers
├── init/               # Database initialization and seed files
├── models/             # Mongoose database models
├── public/             # CSS, JavaScript and static assets
├── routes/             # Application routes
├── utils/              # Utility and helper functions
├── views/              # EJS templates
│
├── app.js              # Main application entry point
├── middleware.js       # Custom middleware
├── schema.js           # Validation schemas
├── package.json
├── .env
└── README.md
```

---

## 🚀 Getting Started

Follow the steps below to run the project locally.

### 1. Clone the Repository

```bash
git clone https://github.com/iharshkaran/wanderlust.git
cd wanderlust
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env` file in the root directory:

```env
MONGO_URL=your_mongodb_connection_string
SECRET=your_session_secret

CLOUD_NAME=your_cloudinary_cloud_name
CLOUD_API_KEY=your_cloudinary_api_key
CLOUD_API_SECRET=your_cloudinary_api_secret
```

> ⚠️ Never commit your `.env` file or expose your API credentials publicly.

### 4. Initialize the Database

If you want to populate the application with sample data, run the available seed scripts:

```bash
node init/index.js
```

Additional seed files can be executed according to your project setup.

### 5. Start the Application

For development:

```bash
npx nodemon app.js
```

Or:

```bash
node app.js
```

The application will be available at:

```text
http://localhost:8080
```

---

## 🔑 Core Functionality

### Authentication

Users can:

* Create an account
* Log in and log out
* Maintain authenticated sessions
* Access protected features
* Manage resources associated with their account

Authentication and session management are handled using Passport.js and MongoDB-backed sessions.

### Listings

Authenticated users can create their own accommodation listings with information such as:

* Title
* Description
* Location
* Price
* Category
* Images

Owners can also update or remove their listings.

### Image Uploads

Property images are uploaded and stored through **Cloudinary**, allowing the application to handle media without relying on local file storage.

### Interactive Maps

Each listing can display its location through an interactive **Leaflet.js** map.

Location information is processed using OpenStreetMap/Nominatim services.

### Categories

Users can quickly discover properties through different categories, making it easier to find stays based on their interests.

### Reviews & Ratings

Users can share their experience by submitting reviews and ratings for listings.

This creates a community-driven way to evaluate properties.

### Dynamic Pricing

The application supports dynamic tax calculation on listing prices, allowing users to switch between the base price and the price including applicable tax.

---

## 📱 Responsive Design

WanderLust is designed to work across different screen sizes, including:

* 💻 Desktop
* 💻 Laptop
* 📱 Tablet
* 📱 Mobile

The interface uses Bootstrap along with custom CSS to maintain a clean and responsive user experience.

---

## 🌐 Deployment

The application can be deployed on cloud hosting platforms such as **Render**.

Typical configuration:

**Build Command**

```bash
npm install
```

**Start Command**

```bash
node app.js
```

Before deploying, configure all required environment variables in the hosting platform.

---

## 🔒 Environment Variables

| Variable           | Description                  |
| ------------------ | ---------------------------- |
| `MONGO_URL`        | MongoDB connection string    |
| `SECRET`           | Secret key used for sessions |
| `CLOUD_NAME`       | Cloudinary cloud name        |
| `CLOUD_API_KEY`    | Cloudinary API key           |
| `CLOUD_API_SECRET` | Cloudinary API secret        |

---

<!-- ## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

To contribute:

```bash
git clone https://github.com/iharshkaran/wanderlust.git
cd wanderlust
npm install
```

Create a new branch, make your changes, and submit a pull request.

---

## 📄 License

This project is licensed under the **MIT License**.

See the `LICENSE` file for details.

--- -->

## 👨‍💻 Author

**Harsh**

If you found this project useful or interesting, consider giving the repository a ⭐.
