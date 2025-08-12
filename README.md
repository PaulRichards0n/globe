# 🌍 Real-Time 3D Earth Globe

An interactive 3D Earth visualization with real-time data feeds for earthquakes, hurricanes, active fires, aircraft tracking, and space station monitoring.

## 🚀 Features

### 🔴 **Earthquake Monitoring**
- Real-time earthquake data from USGS FDSN
- Magnitude-based color coding and sizing
- Multiple data feeds (hourly, daily, weekly, monthly)
- Interactive earthquake details with depth and timing
- Auto-refresh capabilities

### 🌀 **Hurricane & Storm Tracking**
- Current storm positions from NOAA/NHC
- Hurricane warning polygons and alerts
- Real-time storm center markers
- Multi-source data feeds with CORS-aware fetching
- Auto-refresh every 10 minutes

### 🔥 **Active Fire Detection**
- NASA FIRMS (Fire Information for Resource Management System)
- MODIS and VIIRS satellite fire data
- Global 24-hour active fire monitoring
- Confidence-based color coding
- Real-time updates multiple times daily

### ✈️ **Aircraft Tracking**
- Live aircraft positions via OpenSky Network
- Flight path visualization
- Aircraft details on click
- Altitude and speed information

### 🛰️ **International Space Station (ISS)**
- Real-time ISS position tracking
- TLE (Two-Line Element) orbit calculation
- Live altitude and coordinate display
- Orbit path visualization

### 🌏 **Geological Layers**
- Tectonic plate boundaries overlay
- Interactive plate boundary visualization
- Toggle-able geological features

## 🎮 **Interactive Controls**

- **Auto-Update**: Toggle automatic data refreshing
- **Data Feeds**: Switch between time ranges (hour/day/week/month)
- **Layers**: Toggle individual overlays (plates, hurricanes, fires)
- **Zoom & Rotate**: Mouse controls for 3D navigation
- **Click Details**: Click any marker for detailed information

## 🛠️ **Technical Stack**

- **Three.js r128**: 3D graphics and rendering
- **satellite.js v5.0.0**: ISS orbit calculations
- **Vanilla JavaScript**: No frameworks, pure performance
- **WebGL**: Hardware-accelerated 3D graphics
- **Real-time APIs**: USGS, NOAA, NASA, OpenSky Network

## 📊 **Data Sources**

- **USGS**: Earthquake data (earthquake.usgs.gov)
- **NOAA/NHC**: Hurricane and storm data
- **NASA FIRMS**: Active fire detection
- **OpenSky Network**: Aircraft tracking
- **Celestrak**: ISS orbital elements
- **Fraxen**: Tectonic plate boundaries

## 🚀 **Getting Started**

1. **Clone the repository**:
   ```bash
   git clone [your-repo-url]
   cd Shaker
   ```

2. **Start a local server**:
   ```bash
   python -m http.server 8000
   ```

3. **Open in browser**:
   ```
   http://localhost:8000/index.html
   ```

4. **Explore the controls**:
   - Click the ⚙️ button to open controls
   - Toggle different data layers
   - Click on markers for details

## 🔧 **Configuration**

### Update Intervals
- **Earthquakes**: 60 seconds
- **Aircraft**: 30 seconds  
- **ISS**: 10 seconds
- **Hurricanes**: 10 minutes
- **Fires**: 30 minutes

### Performance Optimization
- Fire markers limited to 5,000 for performance
- Automatic cleanup of disposed objects
- Memory management for 3D objects
- Efficient raycasting for interactions

## 🛡️ **Security Features**

- Input sanitization and XSS protection
- CORS-aware API fetching with proxy fallbacks
- Secure URL validation
- Memory cleanup and disposal

## 📱 **Browser Compatibility**

- Modern browsers with WebGL support
- Chrome, Firefox, Safari, Edge
- Mobile-responsive design
- Hardware acceleration recommended

## 🤝 **Contributing**

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📜 **License**

This project is open source. Please respect the terms of service of all data providers.

## 🙏 **Data Provider Attribution**

- **USGS**: Earthquake data courtesy of the U.S. Geological Survey
- **NOAA**: Weather and hurricane data from National Oceanic and Atmospheric Administration
- **NASA**: Fire data from NASA Fire Information for Resource Management System
- **OpenSky Network**: Aircraft data from The OpenSky Network
- **Natural Earth**: Geographic boundary data

## 🐛 **Known Issues**

- Some government APIs may require CORS proxies
- Large datasets may impact performance on slower devices
- Real-time data depends on external API availability

## 📈 **Future Enhancements**

- [ ] Volcanic activity monitoring
- [ ] Weather patterns visualization
- [ ] Ocean current overlays
- [ ] Climate data integration
- [ ] Mobile app version

---

**Built with ❤️ for real-time Earth monitoring**
