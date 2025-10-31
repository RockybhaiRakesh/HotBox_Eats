# Food Billing System 🍽️
A comprehensive, mobile-friendly food billing and order management system built with HTML, CSS, and JavaScript. Perfect for small restaurants, food trucks, or cafes looking for a simple yet powerful billing solution.

# 🌟 Features
# 🛍️ Core Functionality

- Interactive Menu with categorized food items

- Smart Cart System with quantity controls

- Real-time Calculations with tax support

Order Management with local storage persistence

QR Code Generation for order tracking

# 📊 Reporting & Analytics
Sales Reports with date range filtering

Revenue Statistics dashboard

CSV Export for external analysis

Order History with detailed breakdowns

🎨 User Experience
Mobile-First Design responsive across all devices

Dark/Light Theme with modern UI

Toast Notifications for user feedback

Search & Filter functionality

Image Support for menu items

⚙️ Advanced Features
Custom Item Management with image upload

Multiple QR Code Generation methods

Data Backup & Export

Offline Capability (PWA-ready)

🚀 Quick Start
Prerequisites
Modern web browser (Chrome, Firefox, Safari, Edge)

Local server (for image upload features)

Installation
Save the HTML file:

bash
# Save as billing.html
# Open directly in browser or serve via local server
Using Local Server (Recommended):

bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js (if you have http-server installed)
npx http-server

# PHP
php -S localhost:8000
Access the Application:

text
Open http://localhost:8000/billing.html in your browser
📁 File Structure
text
food-billing-system/
│
├── billing.html                 # Main application file
├── README.md                   # This documentation
└── assets/                     # Optional assets folder
    ├── images/                 # Custom food images
    ├── icons/                  # Application icons
    └── exports/                # CSV export location
🎯 Usage Guide
Adding Items to Cart
Browse the categorized menu

Click/Tap on any food item image to add to cart

Adjust quantities using +/- buttons in cart

View real-time total with tax calculation

Managing Orders
Checkout to save orders to browser storage

View QR Code for order tracking

Access reports for sales analytics

Export data as CSV for external use

Customizing Menu
Click "Add Item" button in menu section

Fill details: Name, Price, Category

Upload image (optional)

Save to add to menu

Generating Reports
Select date range using preset buttons or custom dates

Click "Run Report" to view sales data

Export CSV for external analysis

View statistics in dashboard cards

🛠️ Configuration
Tax Rate
Modify the tax rate in the JavaScript section:

javascript
const TAX_RATE = 0.05; // Change to your local tax rate
Currency
Update currency symbol throughout the code:

javascript
// Replace ₹ with your currency symbol
subtotalEl.textContent = `₹${sub.toFixed(2)}`;
Storage Keys
Customize localStorage keys if needed:

javascript
const KEY = 'billing_orders_v2';        // Orders storage
const ITEMS_KEY = 'billing_items_v2';   // Menu items storage
📱 Mobile Optimization
The system is fully optimized for mobile devices with:

Touch-friendly interface elements

Responsive grid layouts

Optimized images for fast loading

Gesture support for cart management

🔧 Technical Details
Browser Compatibility
✅ Chrome 60+

✅ Firefox 55+

✅ Safari 12+

✅ Edge 79+

Storage
LocalStorage for data persistence

~5MB typical storage usage

Automatic backup on checkout

Performance
Fast loading (no external dependencies required)

Efficient rendering with virtual DOM techniques

Optimized images with lazy loading

📊 Data Management
Exporting Data
CSV Export: Complete order history with all details

QR Codes: Individual order information

Browser Backup: Automatic local storage

Clearing Data
Clear Cart: Removes current session items

Clear Orders: Deletes all order history (irreversible)

Reset All: Refresh page to clear temporary data

🎨 Customization
Styling
Modify CSS variables in the :root section:

css
:root {
  --primary: #2b8cff;      /* Main brand color */
  --secondary: #ff6b6b;    /* Accent/error color */
  --success: #4caf50;      /* Success color */
  /* ... more variables */
}
Adding Categories
Update the category list in the add item modal:

html
<select id="newItemCategory">
  <option value="Breakfast">Breakfast</option>
  <option value="Lunch">Lunch</option>
  <!-- Add more categories -->
</select>
🔒 Privacy & Security
No external data sharing

All data stored locally in browser

No tracking or analytics

Offline functionality

🐛 Troubleshooting
Common Issues
Images not loading:

Check internet connection for external images

Use local server for custom image uploads

System will fallback to SVG placeholders

QR Code not generating:

Requires internet for Google Charts API fallback

Canvas method works offline but is basic

Check browser console for errors

Data not persisting:

Ensure cookies/localStorage enabled

Check browser storage limits

Try different browser

Mobile display issues:

Refresh page

Check viewport settings

Ensure responsive design enabled

Debug Mode
Add this to browser console for debugging:

javascript
localStorage.debug = 'true';
📈 Future Enhancements
Planned features for future versions:

Print receipts functionality

Multi-language support

Advanced analytics with charts

Customer management system

Inventory tracking

Multi-user support

Cloud backup integration

API endpoints for external systems

🤝 Contributing
We welcome contributions! Here's how you can help:

Fork the repository

Create a feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add some AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a Pull Request

Development Setup
bash
# Clone the repository
git clone https://github.com/yourusername/food-billing-system.git

# Navigate to directory
cd food-billing-system

# Open in preferred code editor
code .
📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgments
Icons: Font Awesome for beautiful icons

Images: Unsplash for food photography

QR Codes: Google Charts API for QR generation

Inspiration: Various open-source billing systems

📞 Support
Need help? Here are your options:

Check the troubleshooting section above

Create an issue on GitHub

Email support@example.com

Documentation: Visit our wiki

🗺️ Roadmap
Version 2.1.0 (Upcoming)
Receipt printing

Barcode support

Enhanced reports

Version 2.2.0 (Planned)
Customer database

Loyalty program

SMS notifications

Version 3.0.0 (Future)
PWA mobile app

Cloud synchronization

Multi-location support

