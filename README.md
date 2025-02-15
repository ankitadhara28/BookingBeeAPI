# BookingBeeAPI

Welcome to **BookingBeeAPI**! 🐝 This project, maintained by [ankitadhara28](https://github.com/ankitadhara28), is designed to provide hotel booking information with filtering and sorting options through a simple API.

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Endpoints](#endpoints)
  - [GET /hotels](#get-hotels)
  - [GET /hotels/sort/pricing](#get-hotelssortpricing)
  - [GET /hotels/sort/rating](#get-hotelssortrating)
  - [GET /hotels/sort/reviews](#get-hotelssortreviews)
  - [GET /hotels/filter/amenity](#get-hotelsfilteramenity)
  - [GET /hotels/filter/country](#get-hotelsfiltercountry)
  - [GET /hotels/filter/category](#get-hotelsfiltercategory)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## 📜 Project Overview
**BookingBeeAPI** is a Node.js-based REST API that provides a list of hotels and enables sorting and filtering based on various criteria such as pricing, rating, reviews, country, category, and amenities.

## 🌟 Features
- Retrieve a complete list of hotels
- Sort hotels by:
  - Pricing (low-to-high, high-to-low)
  - Rating (low-to-high, high-to-low)
  - Reviews (most-to-least, least-to-most)
- Filter hotels by:
  - Amenity
  - Country
  - Category

## ⚙️ Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ankitadhara28/BookingBeeAPI.git
   ```
2. Navigate to the project directory:
   ```bash
   cd BookingBeeAPI
   ```
3. Install dependencies:
   ```bash
   npm install
   ```

4. Start the server:
   ```bash
   npm start
   ```

The server will start on `http://localhost:3000`.

## 🚀 Usage

### Base URL:
```
http://localhost:3000
```

### 🔗 Endpoints

#### GET /hotels
Returns the complete list of hotels.

Example:
```bash
GET http://localhost:3000/hotels
```

---

#### GET /hotels/sort/pricing
Sorts hotels by pricing.

**Query Parameters:**
- `pricing`: Accepts `low-to-high` or `high-to-low`.

Example:
```bash
GET http://localhost:3000/hotels/sort/pricing?pricing=low-to-high
```

---

#### GET /hotels/sort/rating
Sorts hotels by rating.

**Query Parameters:**
- `rating`: Accepts `low-to-high` or `high-to-low`.

Example:
```bash
GET http://localhost:3000/hotels/sort/rating?rating=high-to-low
```

---

#### GET /hotels/sort/reviews
Sorts hotels by the number of reviews.

**Query Parameters:**
- `reviews`: Accepts `most-to-least` or `least-to-most`.

Example:
```bash
GET http://localhost:3000/hotels/sort/reviews?reviews=most-to-least
```

---

#### GET /hotels/filter/amenity
Filters hotels by amenity.

**Query Parameters:**
- `amenity`: The amenity to filter by (e.g., `Spa`, `Pool`).

Example:
```bash
GET http://localhost:3000/hotels/filter/amenity?amenity=Spa
```

---

#### GET /hotels/filter/country
Filters hotels by country.

**Query Parameters:**
- `country`: The country to filter by (e.g., `India`, `France`).

Example:
```bash
GET http://localhost:3000/hotels/filter/country?country=India
```

---

#### GET /hotels/filter/category
Filters hotels by category.

**Query Parameters:**
- `category`: The category to filter by (e.g., `Luxury`, `Family`).

Example:
```bash
GET http://localhost:3000/hotels/filter/category?category=Luxury
```

## 💻 Technologies Used
- **Node.js**: JavaScript runtime
- **Express**: Web framework for Node.js
- **Cors**: Cross-origin resource sharing

## 🤝 Contributing
Contributions are welcome! If you would like to contribute to this project:
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Create a pull request.

## 📄 License
This project is licensed under the MIT License.

---

Thank you for checking out **BookingBeeAPI**! Feel free to reach out if you have any questions or feedback. 😊

