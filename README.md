

EduPath is a responsive web application designed to help students discover, compare, and evaluate colleges based on their preferences. The application provides an intuitive interface for searching colleges, filtering by budget, comparing multiple institutions, and predicting admission chances based on rank.

The project is built using **HTML**, **Tailwind CSS**, and **Vanilla JavaScript**, with all college data embedded directly in the application, allowing it to run completely offline.


### 🔍 College Search

* Search colleges by name or city.
* Real-time filtering as users type.
* Fast and responsive user experience.

### 💰 Budget Filtering

* Interactive fee range slider.
* Instantly updates the college list based on selected budget.
* Displays active filters dynamically.

### ⚖️ College Comparison

* Add multiple colleges to a comparison list.
* Floating comparison tray for quick access.
* Detailed comparison modal showing:

  * College Name
  * City
  * Fee Structure
  * Cutoff Rank
  * Available Seats
  * Rating

### 🎯 Admission Predictor

* Enter your rank to estimate admission chances.
* Categorizes colleges into:

  * **Likely Colleges** ✅
  * **On the Edge** ⚠️
  * **Unlikely Colleges** ❌
* Provides quick insights for decision-making.

### 📱 Responsive Design

* Optimized for desktop, tablet, and mobile devices.
* Built with Tailwind CSS utility classes.

### 🌐 Offline Support

* No backend or API dependency.
* Embedded dataset allows the application to run locally without internet access.

---

## Technologies Used

* **HTML5**
* **Tailwind CSS**
* **JavaScript (ES6+)**
* **Intl.NumberFormat API** (for Indian currency formatting)

---

## Project Structure

```text
EduPath/
│
├── index.html       # Main application file
├── README.md        # Project documentation
│
└── Assets (optional)
```

---

## Sample Dataset

The application includes data for several colleges such as:

* IIT Madras
* NIT Trichy
* Anna University
* BITS Pilani
* VIT Vellore
* SSN College of Engineering
* PSG College of Technology
* Kumaraguru College of Technology

Each college record contains:

```javascript
{
  id: 1,
  name: "IIT Madras",
  city: "Chennai",
  fee: 50000,
  rankCutoff: 190,
  seats: 120,
  rating: 4.9
}
```

---

## How to Run

### Method 1: Open Directly

1. Download the project files.
2. Open `index.html` in any modern browser.
3. Start exploring colleges immediately.

### Method 2: Local Server

Using VS Code Live Server:

1. Install the Live Server extension.
2. Right-click `index.html`.
3. Select **Open with Live Server**.

---

## Admission Prediction Logic

The predictor compares the student's rank with each college's cutoff rank.

### Categories

**Likely**

```text
Student Rank ≤ College Cutoff
```

**On the Edge**

```text
Student Rank > Cutoff
AND
Difference ≤ 10
```

**Unlikely**

```text
Difference > 10
```

---

## Future Enhancements

* Backend database integration
* Real college admission datasets
* User authentication
* College detail pages
* Advanced filtering options
* Course-wise predictions
* AI-based recommendation system
* Bookmark and save favorite colleges
* Export comparison reports to PDF

---

## Screens

### Home Page

* Search colleges
* Filter by budget
* View available colleges



* Compare selected colleges side-by-side

### Admission Predictor

* Rank-based admission probability analysis

---

## Author

Developed as a College Discovery and Admission Prediction Web Application using modern frontend technologies.

---

## License

This project is open-source and available for educational and learning purposes.
