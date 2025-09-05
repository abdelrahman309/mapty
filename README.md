# 🏃‍♂️ Mapty - Map Your Workouts

A modern, interactive workout tracking application that allows users to log and visualize their fitness activities on an interactive map. Built with vanilla JavaScript, HTML, and CSS.

## 🌐 Live Demo

Visit the live application: [https://mapty-sooty.vercel.app/](https://mapty-sooty.vercel.app/)

## ✨ Features

- **📍 Location-Based Workout Tracking**: Click anywhere on the map to log your workout at that specific location
- **🏃‍♂️ Multiple Workout Types**: Support for running and cycling workouts
- **📊 Detailed Metrics**: Track distance, duration, pace, and cadence/elevation gain
- **🗺️ Interactive Map**: Powered by Leaflet.js for smooth map interactions
- **💾 Local Storage**: All workout data persists locally in your browser
- **📱 Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **🎯 Current Location**: Automatically centers the map on your current location (with permission)

## 🛠️ Technologies Used

- **Frontend**: HTML5, CSS3, Vanilla JavaScript (ES6+)
- **Map Library**: [Leaflet.js](https://leafletjs.com/) - Open-source interactive map library
- **API**: OpenStreetMap tiles for map data
- **Storage**: Browser's localStorage API
- **Deployment**: Vercel

## 🚀 Getting Started

### Prerequisites

- A modern web browser with JavaScript enabled
- Internet connection for map tiles

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/abdelrahman309/mapty.git
   ```

2. Navigate to the project directory:
   ```bash
   cd mapty
   ```

3. Open `index.html` in your web browser or serve it using a local server:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js (if you have live-server installed)
   npx live-server
   ```

4. Visit `http://localhost:8000` in your browser

## 📖 How to Use

1. **Allow Location Access**: When prompted, allow the application to access your location for the best experience

2. **Add a Workout**:
   - Click on any location on the map where you had your workout
   - Fill in the workout form that appears:
     - Select workout type (Running or Cycling)
     - Enter distance (km)
     - Enter duration (minutes)
     - Additional metrics will be calculated automatically

3. **View Your Workouts**:
   - All logged workouts appear in the sidebar
   - Click on any workout in the list to pan to its location on the map
   - Workout markers are color-coded by type

4. **Data Persistence**: Your workouts are automatically saved and will be available when you return to the app

## 🏗️ Project Structure

```
mapty/
├── index.html          # Main HTML file
├── style.css           # Styling and responsive design
├── script.js           # Main application logic
├── icon.png           # Application icon
└── README.md          # Project documentation
```

## 🧩 Key Components

### JavaScript Architecture
- **App Class**: Main application controller
- **Workout Class**: Base class for all workouts
- **Running Class**: Extends Workout with pace calculation
- **Cycling Class**: Extends Workout with speed calculation

### Core Features Implementation
- **Geolocation API**: For getting user's current position
- **Event Handling**: Click events on map and form submissions
- **Local Storage**: Serializing and deserializing workout data
- **DOM Manipulation**: Dynamic rendering of workout list and map markers

## 🌟 Features Breakdown

### Running Workouts
- Tracks: Distance, Duration, Cadence (steps/min)
- Calculates: Pace (min/km)

### Cycling Workouts
- Tracks: Distance, Duration, Elevation Gain (m)
- Calculates: Speed (km/h)

## 📱 Browser Compatibility

- Chrome (recommended)
- Firefox
- Safari
- Edge
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🔮 Future Enhancements

- [ ] Edit and delete workout functionality
- [ ] Workout statistics and analytics
- [ ] Export workout data
- [ ] Social sharing features
- [ ] Weather integration
- [ ] Route planning
- [ ] Additional workout types

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/abdelrahman309/mapty/issues).

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

**Abdelrahman Steit**

- GitHub: [@abdelrahman309](https://github.com/abdelrahman309)
- LinkedIn: [abdelrahman-steit](https://linkedin.com/in/abdelrahman-steit)

## 🙏 Acknowledgments

- Map tiles provided by [OpenStreetMap](https://www.openstreetmap.org/)
- Interactive maps powered by [Leaflet.js](https://leafletjs.com/)
- Inspiration from fitness tracking applications

---

⭐ If you found this project helpful, please give it a star!
