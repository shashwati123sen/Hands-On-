# HandsOn - Frontend

## 📌 Project Overview
HandsOn is a community-driven social volunteering platform that connects individuals with meaningful social impact opportunities. This repository contains the **React.js frontend**, allowing users to:

- Create and manage volunteer events
- Browse and filter public event listings
- Instantly register for events with a single click
- Post and respond to community help requests

## 🚀 Features Implemented

### 1️⃣ Event Management
- **Event Creation**: Users or organizations can create volunteer events by providing details such as title, description, date, time, location, and category.
- **Event Listing & Filters**: Users can browse upcoming volunteer events and filter them by category, location, and availability.
- **One-Click Registration**: Users can instantly join an event, which adds them to the attendee list.

### 2️⃣ Event & Post Differentiation
- **Events**: Fixed time and date for participation.
- **Community Help Posts**: Open-ended requests for ongoing support (e.g., "Need volunteers to tutor weekly").

### 3️⃣ Community Help Requests
- **Users & Organizations can post requests for help** (e.g., “We need volunteers to distribute winter clothes to homeless people.”).
- **Others can offer help** through comments or private messaging.
- **Urgency Levels**: Requests can be marked as low, medium, or urgent to prioritize responses.
- **Dynamic Help Request Board**: Community members can proactively offer assistance.

## 🛠️ Tech Stack
- **Frontend**: React.js (with React Router for navigation)
- **State Management**: Context API / Redux (optional)
- **Styling**: Tailwind CSS / Styled Components
- **API Communication**: Axios (REST API calls)
- **Authentication**: JWT-based authentication (if implemented)

## 📂 Project Structure
```
frontend/
│── public/
│── src/
│   ├── components/  # Reusable components
│   ├── pages/        # Page components
│   ├── services/     # API calls
│   ├── context/      # State management (if used)
│   ├── utils/        # Helper functions
│   ├── App.js        # Main app component
│   ├── index.js      # Entry point
│── package.json
│── README.md
```

## 🔧 Setup & Installation

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/hands-on-frontend.git
cd hands-on-frontend
```

### 2️⃣ Install Dependencies
```bash
npm install  # or yarn install
```

### 3️⃣ Run the Development Server
```bash
npm start  # or yarn start
```
The application will be available at `http://localhost:3000/`.

## 🚀 API Integration
Ensure the backend API is running and update the API endpoints in the service files.

Example API Configuration (`src/services/api.js`):
```javascript
import axios from 'axios';

const API_BASE_URL = 'http://localhost:5000/api';

export const fetchEvents = async () => {
    return await axios.get(`${API_BASE_URL}/events`);
};
```

## 📝 Contribution Guidelines
1. **Fork** the repository.
2. Create a **feature branch** (`feature/your-feature-name`).
3. **Commit** your changes (`git commit -m 'Add new feature'`).
4. **Push** to the branch (`git push origin feature/your-feature-name`).
5. Submit a **Pull Request**.

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

🎯 **Happy Coding & Volunteering!** 🚀
