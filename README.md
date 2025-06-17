<<<<<<< HEAD
# Solar Market Trend Analyzer

A comprehensive web application for analyzing solar, inverter, and battery market trends using real-time data scraping and API integrations.

## 🚀 Quick Start

### Option 1: Full Setup with Backend (Recommended)

1. **Install Node.js** (if not installed)

   - Download from [nodejs.org](https://nodejs.org/)
   - Verify installation: `node --version`

2. **Create Project Directory**

   ```bash
   mkdir solar-market-analyzer
   cd solar-market-analyzer
   ```

3. **Save Files**

   - Save `package.json` in the project directory
   - Save `server.js` (the backend code) in the project directory
   - Create a `public` folder and save the HTML file as `public/index.html`

4. **Install Dependencies**

   ```bash
   npm install
   ```

5. **Start the Server**

   ```bash
   npm start
   ```

6. **Open in Browser**
   - Go to `http://localhost:3000`
   - The app will work with both real APIs and fallback data

### Option 2: Frontend Only (No Backend Required)

Simply open the HTML file directly in your browser. The app will automatically use demo data and still provide full functionality for presentations.

## 🔧 Configuration

### API Keys (Optional - Free Tiers Available)

To enable real data sources, sign up for these free APIs:

1. **NewsAPI** (newsapi.org) - 1000 requests/month free
2. **Alpha Vantage** (alphavantage.co) - 5 API calls/minute free
3. **OpenWeatherMap** (openweathermap.org) - 1000 calls/day free
4. **Polygon.io** (polygon.io) - 5 API calls/minute free

Add your API keys to the server.js file:

```javascript
const NEWS_API_KEY = "your-news-api-key";
const ALPHA_VANTAGE_KEY = "your-alpha-vantage-key";
// etc.
```

### Environment Variables (Optional)

Create a `.env` file:

```
PORT=3000
NEWS_API_KEY=your-key-here
ALPHA_VANTAGE_KEY=your-key-here
OPENWEATHER_API_KEY=your-key-here
```

## 📊 Features

### Data Sources

- **News APIs**: Solar industry news and updates
- **Reddit**: Community discussions and sentiment
- **Stock APIs**: Solar company stock prices
- **Weather APIs**: Solar efficiency calculations
- **Web Scraping**: Industry websites and reports

### Analysis Capabilities

- Price trend monitoring
- Market sentiment analysis
- Volume tracking
- Regional comparisons
- Custom keyword alerts
- Trend forecasting

### Export Options

- CSV data export
- Real-time updates
- Historical data tracking

## 🌐 API Endpoints

When the backend is running:

- `GET /api/analyze` - Start market analysis
- `GET /api/trends` - Get trend analysis
- `GET /api/export` - Export data as CSV
- `GET /api/status` - Check server status

## 🛠️ Customization

### Adding New Data Sources

1. **Add to server.js**:

   ```javascript
   async fetchCustomSource() {
       // Your scraping logic here
   }
   ```

2. **Update analysis function**:
   ```javascript
   const results = await Promise.allSettled([
     this.fetchNewsData(category),
     this.fetchCustomSource(), // Add here
     // ... other sources
   ]);
   ```

### Custom Keywords

Add industry-specific keywords in server.js:

```javascript
const SOLAR_KEYWORDS = [
  "your-custom-keyword",
  "specific-product-name",
  // ... existing keywords
];
```

## 🔍 Troubleshooting

### Common Issues

1. **"Failed to fetch" Error**

   - Backend server not running: `npm start`
   - Port conflict: Change PORT in server.js
   - CORS issues: Server handles this automatically

2. **No Real Data Showing**

   - API keys not configured: Add keys to server.js
   - Rate limits exceeded: Wait or use different APIs
   - Network issues: App falls back to demo data

3. **Module Not Found**
   - Run `npm install` to install dependencies
   - Check Node.js version: `node --version`

### Development Mode

```bash
npm run dev  # Auto-restart on file changes
```

## 📈 Scaling for Production

### Database Integration

- Add MongoDB or PostgreSQL for data persistence
- Implement data caching with Redis
- Add user authentication

### Advanced Features

- Real-time WebSocket updates
- Advanced chart visualizations
- Email/SMS alerts for price changes
- Machine learning trend predictions

### Deployment Options

- **Heroku**: Easy deployment with free tier
- **DigitalOcean**: VPS hosting
- **AWS/Azure**: Enterprise scaling
- **Netlify**: Frontend-only deployment

## 🚨 Rate Limits & Costs

### Free API Limits

- NewsAPI: 1,000 requests/month
- Alpha Vantage: 5 calls/minute, 500/day
- OpenWeatherMap: 1,000 calls/day
- Reddit: No official limits (be respectful)

### Upgrade Paths

Most APIs offer paid tiers for higher limits:

- NewsAPI: $449/month for unlimited
- Alpha Vantage: $49.99/month for premium
- Consider rotating multiple free API keys

## 📝 License

Bsc License - Feel free to customize for your business needs.

## 🆘 Support

For technical support:

1. Check the troubleshooting section
2. Verify all dependencies are installed
3. Check browser console for errors
4. Ensure backend server is running

The application is designed to work even without the backend server, providing demo data for presentations and testing.
=======
# Solar Market Trend Analyzer

A comprehensive web application for analyzing solar, inverter, and battery market trends using real-time data scraping and API integrations.

## 🚀 Quick Start

### Option 1: Full Setup with Backend (Recommended)

1. **Install Node.js** (if not installed)

   - Download from [nodejs.org](https://nodejs.org/)
   - Verify installation: `node --version`

2. **Create Project Directory**

   ```bash
   mkdir solar-market-analyzer
   cd solar-market-analyzer
   ```

3. **Save Files**

   - Save `package.json` in the project directory
   - Save `server.js` (the backend code) in the project directory
   - Create a `public` folder and save the HTML file as `public/index.html`

4. **Install Dependencies**

   ```bash
   npm install
   ```

5. **Start the Server**

   ```bash
   npm start
   ```

6. **Open in Browser**
   - Go to `http://localhost:3000`
   - The app will work with both real APIs and fallback data

### Option 2: Frontend Only (No Backend Required)

Simply open the HTML file directly in your browser. The app will automatically use demo data and still provide full functionality for presentations.

## 🔧 Configuration

### API Keys (Optional - Free Tiers Available)

To enable real data sources, sign up for these free APIs:

1. **NewsAPI** (newsapi.org) - 1000 requests/month free
2. **Alpha Vantage** (alphavantage.co) - 5 API calls/minute free
3. **OpenWeatherMap** (openweathermap.org) - 1000 calls/day free
4. **Polygon.io** (polygon.io) - 5 API calls/minute free

Add your API keys to the server.js file:

```javascript
const NEWS_API_KEY = "your-news-api-key";
const ALPHA_VANTAGE_KEY = "your-alpha-vantage-key";
// etc.
```

### Environment Variables (Optional)

Create a `.env` file:

```
PORT=3000
NEWS_API_KEY=your-key-here
ALPHA_VANTAGE_KEY=your-key-here
OPENWEATHER_API_KEY=your-key-here
```

## 📊 Features

### Data Sources

- **News APIs**: Solar industry news and updates
- **Reddit**: Community discussions and sentiment
- **Stock APIs**: Solar company stock prices
- **Weather APIs**: Solar efficiency calculations
- **Web Scraping**: Industry websites and reports

### Analysis Capabilities

- Price trend monitoring
- Market sentiment analysis
- Volume tracking
- Regional comparisons
- Custom keyword alerts
- Trend forecasting

### Export Options

- CSV data export
- Real-time updates
- Historical data tracking

## 🌐 API Endpoints

When the backend is running:

- `GET /api/analyze` - Start market analysis
- `GET /api/trends` - Get trend analysis
- `GET /api/export` - Export data as CSV
- `GET /api/status` - Check server status

## 🛠️ Customization

### Adding New Data Sources

1. **Add to server.js**:

   ```javascript
   async fetchCustomSource() {
       // Your scraping logic here
   }
   ```

2. **Update analysis function**:
   ```javascript
   const results = await Promise.allSettled([
     this.fetchNewsData(category),
     this.fetchCustomSource(), // Add here
     // ... other sources
   ]);
   ```

### Custom Keywords

Add industry-specific keywords in server.js:

```javascript
const SOLAR_KEYWORDS = [
  "your-custom-keyword",
  "specific-product-name",
  // ... existing keywords
];
```

## 🔍 Troubleshooting

### Common Issues

1. **"Failed to fetch" Error**

   - Backend server not running: `npm start`
   - Port conflict: Change PORT in server.js
   - CORS issues: Server handles this automatically

2. **No Real Data Showing**

   - API keys not configured: Add keys to server.js
   - Rate limits exceeded: Wait or use different APIs
   - Network issues: App falls back to demo data

3. **Module Not Found**
   - Run `npm install` to install dependencies
   - Check Node.js version: `node --version`

### Development Mode

```bash
npm run dev  # Auto-restart on file changes
```

## 📈 Scaling for Production

### Database Integration

- Add MongoDB or PostgreSQL for data persistence
- Implement data caching with Redis
- Add user authentication

### Advanced Features

- Real-time WebSocket updates
- Advanced chart visualizations
- Email/SMS alerts for price changes
- Machine learning trend predictions

### Deployment Options

- **Heroku**: Easy deployment with free tier
- **DigitalOcean**: VPS hosting
- **AWS/Azure**: Enterprise scaling
- **Netlify**: Frontend-only deployment

## 🚨 Rate Limits & Costs

### Free API Limits

- NewsAPI: 1,000 requests/month
- Alpha Vantage: 5 calls/minute, 500/day
- OpenWeatherMap: 1,000 calls/day
- Reddit: No official limits (be respectful)

### Upgrade Paths

Most APIs offer paid tiers for higher limits:

- NewsAPI: $449/month for unlimited
- Alpha Vantage: $49.99/month for premium
- Consider rotating multiple free API keys

## 📝 License

Bsc License - Feel free to customize for your business needs.

## 🆘 Support

For technical support:

1. Check the troubleshooting section
2. Verify all dependencies are installed
3. Check browser console for errors
4. Ensure backend server is running

The application is designed to work even without the backend server, providing demo data for presentations and testing.
>>>>>>> 3fa2565 (again API)
