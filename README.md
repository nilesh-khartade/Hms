# HospitalCare Management System

A comprehensive, modern hospital management system built with HTML, CSS, and JavaScript. This system provides a complete solution for managing patients, doctors, appointments, and medical inventory in a hospital setting.

## 🏥 Project Overview

HospitalCare is a full-featured hospital management system that enables healthcare facilities to:
- Manage patient records and medical histories
- Schedule and track appointments
- Maintain doctor profiles and schedules
- Monitor medical inventory and supplies
- Generate reports and analytics
- Visualize data through interactive charts

## ✨ Currently Implemented Features

### 📊 Dashboard Module
- **Real-time Statistics**: Total patients, today's appointments, active doctors, low stock alerts
- **Interactive Charts**: Monthly appointment trends, patient demographics breakdown
- **Quick Actions**: Direct access to all major modules
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices

### 👥 Patient Management
- **Complete Patient Records**: Personal information, medical history, allergies, medications
- **Advanced Search**: Search patients by name, ID, or other criteria
- **Status Tracking**: Active, inactive, transferred patient statuses
- **Data Validation**: Email, phone number, and required field validation
- **Patient Profiles**: Detailed view with edit capabilities

### 📅 Appointment Scheduling
- **Flexible Scheduling**: Date/time selection with doctor availability
- **Appointment Types**: Consultation, follow-up, emergency, surgery, check-up
- **Status Management**: Scheduled → Confirmed → In Progress → Completed workflow
- **Real-time Updates**: Live appointment status changes
- **Calendar View**: Daily appointment overview with filtering

### 👨‍⚚ Doctor Management
- **Doctor Profiles**: Specialization, education, experience, contact information
- **Department Organization**: Cardiology, neurology, pediatrics, etc.
- **Schedule Management**: Working hours and availability
- **Fee Structure**: Consultation fees and pricing
- **Performance Tracking**: Appointment history and patient feedback

### 📦 Inventory Management
- **Medical Supplies Tracking**: Medicines, equipment, supplies, instruments
- **Stock Monitoring**: Current stock, minimum levels, restock alerts
- **Expiry Management**: Expiration date tracking with warnings
- **Cost Tracking**: Unit prices, total inventory value
- **Batch Management**: Lot numbers, supplier information
- **Automatic Status Updates**: In stock, low stock, out of stock, expired

### 🔧 Core System Features
- **RESTful API Integration**: Complete CRUD operations for all modules
- **Real-time Data Sync**: Automatic updates across all components
- **Responsive UI**: Mobile-first design with Tailwind CSS
- **Interactive Charts**: Chart.js integration for data visualization
- **Form Validation**: Client-side validation with error handling
- **Search & Filter**: Advanced search capabilities across all modules
- **Modal System**: Clean, accessible modal dialogs
- **Notification System**: Success, error, and warning notifications

## 🛠 Technology Stack

### Frontend Framework
- **HTML5**: Semantic markup with accessibility features
- **CSS3**: Modern styling with Flexbox and Grid
- **Tailwind CSS**: Utility-first CSS framework
- **JavaScript ES6+**: Modern JavaScript with async/await

### Libraries & Dependencies
- **Chart.js**: Interactive charts and data visualization
- **Font Awesome**: Professional icon library
- **Google Fonts (Inter)**: Modern, readable typography

### Data Management
- **RESTful Table API**: Complete database operations
- **Client-side State Management**: Efficient data caching and updates
- **Real-time Validation**: Form validation and error handling

## 📁 Project Structure

```
hospital-management-system/
├── index.html              # Main application file
├── css/
│   └── style.css          # Custom styles and theme
├── js/
│   ├── main.js           # Core application logic
│   ├── patients.js       # Patient management module
│   ├── appointments.js   # Appointment scheduling module
│   ├── doctors.js        # Doctor management module
│   ├── inventory.js      # Inventory management module
│   └── charts.js         # Charts and data visualization
└── README.md             # Project documentation
```

## 🗄 Database Schema

### Patients Table
- **Personal Info**: First name, last name, date of birth, gender
- **Contact**: Phone, email, address, emergency contact
- **Medical**: Blood type, allergies, medical history, medications
- **Insurance**: Insurance information and policy details
- **Status**: Active, inactive, transferred
- **Timestamps**: Registration date, last updated

### Doctors Table
- **Professional Info**: Name, specialization, license number, department
- **Experience**: Years of experience, education background
- **Contact**: Phone, email, room number
- **Schedule**: Working hours and availability
- **Financial**: Consultation fees
- **Status**: Active, on leave, retired

### Appointments Table
- **Scheduling**: Patient ID, doctor ID, date/time, duration
- **Details**: Reason, type, priority level, room assignment
- **Status**: Scheduled, confirmed, in progress, completed, cancelled, no-show
- **Notes**: Additional appointment notes and instructions
- **Audit**: Created by, updated by, timestamps

### Inventory Table
- **Item Info**: Name, code, category, subcategory, manufacturer
- **Stock**: Quantity, unit, minimum stock level, location
- **Financial**: Unit price, total value
- **Expiry**: Expiration date, batch number
- **Status**: In stock, low stock, out of stock, expired, recalled
- **Supply Chain**: Supplier information, last restocked date

## 🚀 API Endpoints

### RESTful Table API Operations
All modules use standardized REST API endpoints:

- **GET /tables/{table}** - List records with pagination and search
- **GET /tables/{table}/{id}** - Get single record by ID  
- **POST /tables/{table}** - Create new record
- **PUT /tables/{table}/{id}** - Update existing record (full update)
- **PATCH /tables/{table}/{id}** - Partial record update
- **DELETE /tables/{table}/{id}** - Delete record (soft delete)

### Query Parameters
- `page` - Page number for pagination (default: 1)
- `limit` - Number of records per page (default: 10-100)
- `search` - Search term for filtering records
- `sort` - Field to sort by
- `filter` - Additional filtering criteria

## 🎯 Key Functional Entry Points

### Dashboard (`/`)
- **Statistics Overview**: Real-time counts and metrics
- **Chart Visualization**: Monthly trends and demographics
- **Quick Navigation**: Direct access to all modules

### Patient Management (`/patients`)
- **Patient Registration**: Add new patients with complete profiles
- **Patient Search**: Find patients by name, ID, or other criteria
- **Medical Records**: View and update patient medical information
- **Patient Status**: Manage active/inactive patient statuses

### Appointment Scheduling (`/appointments`)
- **Schedule Appointments**: Date/time selection with doctor availability
- **Appointment Management**: Update status, reschedule, or cancel
- **Calendar View**: Daily/weekly appointment overview
- **Appointment Types**: Different appointment categories and priorities

### Doctor Management (`/doctors`)
- **Doctor Profiles**: Complete professional and contact information
- **Schedule Management**: Working hours and availability tracking
- **Department Organization**: Categorization by medical specialization
- **Performance Metrics**: Appointment history and patient feedback

### Inventory Management (`/inventory`)
- **Stock Tracking**: Current inventory levels and locations
- **Restock Management**: Add inventory with batch tracking
- **Expiry Monitoring**: Automatic alerts for expiring items
- **Cost Analysis**: Inventory valuation and financial reporting

## 🔍 Search and Filter Capabilities

### Global Search Features
- **Patient Search**: Name, email, phone, patient ID
- **Doctor Search**: Name, specialization, department
- **Appointment Search**: Patient name, doctor name, date range
- **Inventory Search**: Item name, category, supplier, location

### Advanced Filtering
- **Status Filters**: Active/inactive patients, appointment statuses
- **Date Filters**: Date ranges for appointments and inventory
- **Category Filters**: Medical departments, inventory categories
- **Stock Filters**: Low stock, expired items, out of stock

## 📈 Reporting and Analytics

### Dashboard Analytics
- **Patient Statistics**: Total patients, new registrations, demographics
- **Appointment Metrics**: Daily appointments, completion rates, trends
- **Doctor Performance**: Active doctors, department distribution
- **Inventory Status**: Stock levels, low stock alerts, expiry warnings

### Data Visualizations
- **Line Charts**: Monthly appointment trends over time
- **Doughnut Charts**: Patient age demographics distribution
- **Bar Charts**: Department-wise doctor distribution
- **Status Charts**: Inventory status breakdown

## 🛡 Data Validation and Security

### Client-Side Validation
- **Required Fields**: Comprehensive validation for all required inputs
- **Format Validation**: Email addresses, phone numbers, dates
- **Range Validation**: Numeric fields with minimum/maximum values
- **Custom Validation**: Medical-specific field validation

### Data Integrity
- **Referential Integrity**: Patient-appointment-doctor relationships
- **Status Consistency**: Automatic status updates based on business rules
- **Audit Trails**: Created/updated timestamps and user tracking
- **Soft Deletes**: Data preservation with deletion flags

## 🚧 Features Not Yet Implemented

### Advanced Features (Future Development)
- **User Authentication**: Login system with role-based access control
- **Multi-tenant Support**: Multiple hospital/clinic management
- **Advanced Reporting**: PDF report generation and export
- **Email Integration**: Appointment reminders and notifications
- **SMS Notifications**: Patient appointment confirmations
- **Barcode Scanning**: Inventory management with barcode support
- **Payment Processing**: Billing and payment tracking integration
- **Lab Results**: Laboratory test results management
- **Prescription Management**: Digital prescription creation and tracking
- **Emergency Management**: Emergency protocols and alert systems

### Technical Enhancements (Recommended Next Steps)
- **Offline Support**: Progressive Web App (PWA) capabilities
- **Real-time Sync**: WebSocket integration for live updates
- **Mobile App**: React Native or Flutter mobile application
- **Print Functionality**: Patient reports, appointment confirmations
- **Data Export**: CSV, Excel, PDF export capabilities
- **Backup System**: Automated data backup and recovery
- **API Rate Limiting**: Request throttling and security
- **Advanced Analytics**: Machine learning insights and predictions

## 🎯 Recommended Next Development Steps

### Phase 1: Core Enhancements (Priority: High)
1. **User Authentication System**
   - Login/logout functionality
   - Role-based permissions (Admin, Doctor, Nurse, Receptionist)
   - Session management and security

2. **Advanced Search and Filtering**
   - Global search across all modules
   - Advanced filter combinations
   - Saved search preferences

3. **Report Generation**
   - PDF report creation
   - Appointment summaries
   - Inventory reports
   - Patient medical records

### Phase 2: Integration Features (Priority: Medium)
1. **Email/SMS Notifications**
   - Appointment reminders
   - Low stock alerts
   - System notifications

2. **Payment Integration**
   - Billing management
   - Payment tracking
   - Invoice generation

3. **Print Functionality**
   - Patient information sheets
   - Appointment confirmations
   - Inventory reports

### Phase 3: Advanced Analytics (Priority: Low)
1. **Business Intelligence**
   - Advanced analytics dashboard
   - Predictive analytics
   - Performance metrics

2. **Mobile Application**
   - Native mobile app
   - Push notifications
   - Offline functionality

3. **Third-party Integrations**
   - Laboratory systems
   - Pharmacy management
   - Insurance verification

## 🏗 System Architecture

### Client-Side Architecture
- **Modular Design**: Separate JavaScript modules for each feature
- **State Management**: Centralized application state with HospitalApp object
- **API Layer**: Abstracted API service for all backend communications
- **UI Components**: Reusable modal, form, and table components

### Data Flow
1. **User Interaction**: Form submissions, button clicks, search inputs
2. **Validation Layer**: Client-side validation and error handling  
3. **API Service**: RESTful API calls with error handling
4. **State Update**: Local state updates and UI refresh
5. **User Feedback**: Success/error notifications and visual updates

### Responsive Design Strategy
- **Mobile-First**: Designed for mobile devices first, then scaled up
- **Breakpoint System**: Tailwind CSS responsive breakpoints
- **Touch-Friendly**: Large touch targets and gesture support
- **Performance**: Optimized for various device capabilities

## 📱 Browser Compatibility

### Supported Browsers
- **Chrome**: Version 80+ (recommended)
- **Firefox**: Version 75+
- **Safari**: Version 13+
- **Edge**: Version 80+

### Mobile Support
- **iOS Safari**: iOS 12+
- **Chrome Mobile**: Android 8+
- **Samsung Internet**: Version 10+

## 🚀 Getting Started

### Prerequisites
- Modern web browser with JavaScript enabled
- Internet connection for CDN resources (Tailwind CSS, Font Awesome, Chart.js)

### Installation
1. Open `index.html` in a web browser
2. The system will automatically initialize with sample data
3. Navigate between modules using the top navigation
4. Add, edit, and manage hospital data through the interface

### Sample Data
The system includes sample data for demonstration:
- **2 Sample Patients**: John Doe and Sarah Johnson
- **2 Sample Doctors**: Dr. Michael Smith (Cardiology) and Dr. Emily Brown (Pediatrics)  
- **2 Sample Inventory Items**: Paracetamol and Surgical Gloves

### Configuration
- No additional configuration required
- Sample data loads automatically on first visit
- All data persists in the session state

## 🤝 Contributing

### Development Guidelines
- Follow existing code structure and naming conventions
- Add comments for complex functionality
- Test all features across different screen sizes
- Validate all forms and handle errors gracefully

### Code Style
- Use ES6+ JavaScript features
- Follow semantic HTML structure
- Use Tailwind CSS utility classes
- Maintain consistent indentation (2 spaces)

## 📄 License

This project is provided as-is for educational and demonstration purposes. Feel free to use, modify, and distribute according to your needs.

---

**HospitalCare Management System** - Building better healthcare through technology 🏥✨