# 🏥 MediMap Care - Find Healthcare Near You

> **Making healthcare accessible and efficient for everyone in Kenya and beyond.**

MediMap Care is a comprehensive healthcare platform that connects patients with verified medical facilities through location-based services, instant appointment booking, and transparent reviews. Built with modern web technologies and designed for the Kenyan healthcare ecosystem.

## 🎯 **Project Overview**

### **Mission Statement**
To revolutionize healthcare access by providing a seamless digital platform that connects patients with quality healthcare providers, eliminating barriers of distance, time, and information.

### **Problem We Solve**
- **Limited Healthcare Access**: Difficulty finding nearby, affordable clinics
- **Manual Booking Processes**: Time-consuming appointment scheduling
- **Lack of Transparency**: Limited visibility into clinic quality and availability
- **Geographic Barriers**: Healthcare deserts in rural and underserved areas

### **Our Solution**
A comprehensive digital health platform featuring:
- 🗺️ **Interactive Maps** with real-time clinic locations
- 📅 **Instant Appointment Booking** with confirmation notifications
- ⭐ **Verified Reviews** and ratings system
- 🔍 **Advanced Search** by specialty, location, and availability
- 📱 **Mobile-First Design** for accessibility anywhere

## ✨ **Key Features**

### **🗺️ Location-Based Discovery**
- **Real-time Geolocation**: Automatic detection of user location
- **Interactive Maps**: OpenStreetMap integration with custom styling
- **Radius Search**: Find clinics within specified distance
- **Kenya Coverage**: Comprehensive coverage of major cities and towns

### **📅 Appointment Management**
- **Instant Booking**: Real-time availability checking
- **Multiple Appointment Types**: In-person and video consultations
- **Smart Scheduling**: Conflict detection and rescheduling
- **Notification System**: Email and SMS confirmations

### **⭐ Review & Rating System**
- **Verified Reviews**: Authentic patient feedback
- **Star Ratings**: 5-star rating system
- **Specialty Reviews**: Detailed feedback by medical specialty
- **Community Validation**: Peer-reviewed clinic information

### **🔍 Advanced Search & Filtering**
- **Specialty Search**: General Practice, Pediatrics, Cardiology, etc.
- **Availability Filters**: Open now, Today, This week
- **Distance Controls**: Customizable search radius
- **Price Range**: Consultation fee filtering

### **👤 User Management**
- **Dual Registration**: Patients and Clinics
- **Profile Management**: Comprehensive user profiles
- **Medical History**: Secure health information storage
- **Emergency Contacts**: Safety and accessibility features

## 🛠️ **Technology Stack**

### **Frontend**
- **React 18** - Modern UI framework with hooks
- **TypeScript** - Type-safe development
- **Vite** - Lightning-fast build tool
- **Tailwind CSS** - Utility-first styling
- **shadcn/ui** - Accessible component library

### **Backend**
- **Node.js** - JavaScript runtime
- **Express.js** - Web application framework
- **TypeScript** - Type-safe backend development
- **PostgreSQL** - Relational database
- **Sequelize** - ORM for database operations
- **JWT** - Authentication tokens
- **bcrypt** - Password hashing

### **Mapping & Location**
- **Leaflet.js** - Interactive mapping library
- **OpenStreetMap** - Free, open-source map tiles
- **React Leaflet** - React integration for maps
- **HTML5 Geolocation** - User location detection

### **State Management**
- **TanStack Query** - Server state management
- **React Context** - Global state management
- **React Hook Form** - Form state and validation
- **Zod** - Schema validation

### **Development Tools**
- **ESLint** - Code linting and formatting
- **TypeScript** - Static type checking
- **PostCSS** - CSS processing
- **Autoprefixer** - Cross-browser compatibility
- **Concurrently** - Run multiple processes simultaneously

## 🏗️ **Project Structure**

```
medimap-care/
├── frontend/              # React TypeScript frontend
│   ├── src/
│   │   ├── components/    # Reusable UI components
│   │   │   ├── dashboard/ # Dashboard-specific components
│   │   │   ├── landing/   # Landing page components
│   │   │   ├── map/       # Map-related components
│   │   │   └── ui/        # Base UI components
│   │   ├── pages/         # Application pages
│   │   │   ├── dashboard/ # Dashboard pages
│   │   │   ├── Landing.tsx # Homepage
│   │   │   ├── Login.tsx   # Authentication
│   │   │   └── Signup.tsx  # User registration
│   │   ├── services/      # API and utility services
│   │   ├── hooks/         # Custom React hooks
│   │   ├── lib/           # Utility functions
│   │   └── types/         # TypeScript type definitions
│   ├── public/            # Static assets
│   ├── package.json       # Frontend dependencies
│   └── vite.config.ts     # Vite configuration
├── backend/               # Express TypeScript backend
│   ├── src/
│   │   ├── routes/        # API route handlers
│   │   ├── models/        # Database models
│   │   ├── controllers/   # Business logic
│   │   ├── middleware/    # Express middleware
│   │   └── app.ts         # Main application setup
│   ├── package.json       # Backend dependencies
│   └── tsconfig.json      # TypeScript configuration
├── shared/                # Shared types and interfaces
├── package.json           # Root workspace configuration
└── README.md              # Project documentation
```

## 🚀 **Getting Started**

### **Prerequisites**
- Node.js 18+ and npm
- PostgreSQL database (local or cloud)
- Modern web browser with geolocation support
- Internet connection for map tiles

### **Installation**

```bash
# Clone the repository
git clone https://github.com/your-username/medimap-care.git

# Navigate to project directory
cd medimap-care

# Install all dependencies (frontend, backend, root)
npm install

# Set up environment variables
cp backend/.env.example backend/.env
# Edit backend/.env with your database URL and JWT secret

# Start both frontend and backend in development
npm run dev

# Or run them separately:
npm run dev:frontend  # Frontend only
npm run dev:backend   # Backend only
```

### **Environment Setup**

Create `backend/.env` file:
```env
NODE_ENV=development
PORT=8001
DATABASE_URL=postgresql://username:password@localhost:5432/medimap_dev
JWT_SECRET=your-super-secret-jwt-key
JWT_EXPIRES_IN=7d
EMAIL_USER=your-email@gmail.com
EMAIL_PASS=your-email-password
TWILIO_SID=your-twilio-sid
TWILIO_AUTH_TOKEN=your-twilio-token
TWILIO_PHONE_NUMBER=+1234567890
```

### **Database Setup**

```bash
# Navigate to backend
cd backend

# Run database migrations
npm run migrate

# Seed initial data (optional)
npm run seed
```

### **Development Commands**

```bash
# Root level commands (run both services)
npm run dev              # Start frontend and backend concurrently
npm run build            # Build both frontend and backend
npm run lint             # Lint both projects

# Frontend commands
npm run dev:frontend     # Start frontend only
cd frontend && npm run dev
cd frontend && npm run build
cd frontend && npm run lint

# Backend commands
npm run dev:backend      # Start backend only
cd backend && npm run dev
cd backend && npm run build
cd backend && npm run test
```

## 🌍 **Kenya Healthcare Integration**

### **Geographic Coverage**
- **Primary Cities**: Nairobi, Mombasa, Kisumu, Nakuru, Eldoret
- **Rural Areas**: Major towns and healthcare facilities
- **Transportation**: Matatu routes and accessibility considerations
- **Languages**: English and Swahili support

### **Healthcare Ecosystem**
- **Public Hospitals**: Government health facilities
- **Private Clinics**: Licensed private healthcare providers
- **Specialized Care**: Cardiology, Pediatrics, Maternity
- **Emergency Services**: 24/7 emergency care facilities

## 📱 **Mobile-First Design**

### **Responsive Features**
- **Touch-Optimized**: Mobile-friendly interactions
- **Offline Support**: Basic functionality without internet
- **Progressive Web App**: Installable on mobile devices
- **Accessibility**: Screen reader and keyboard navigation

## 🔒 **Privacy & Security**

### **Data Protection**
- **Location Privacy**: Clear consent and data handling
- **Medical Data**: HIPAA-compliant information storage
- **Secure Communication**: HTTPS for all data transmission
- **User Consent**: Transparent data collection practices

## 🎨 **Design System**

### **Brand Identity**
- **Primary Color**: Medical Teal (#10B981)
- **Secondary Color**: Healthcare Green (#059669)
- **Accent Color**: Warm Coral (#F59E0B)
- **Typography**: Inter font family for readability

### **Visual Elements**
- **Custom Logo**: Medical cross with location pin
- **Gradient Themes**: Healthcare-focused color schemes
- **Smooth Animations**: Professional micro-interactions
- **Dark Mode**: Consistent theming across modes

## 🚀 **Deployment**

### **Production Deployment**
- **Vercel**: Frontend hosting and deployment
- **Netlify**: Alternative hosting platform
- **GitHub Pages**: Static site hosting
- **Custom Domain**: Professional domain integration

### **Environment Variables**
```env
VITE_APP_NAME=MediMap Care
VITE_APP_URL=https://medimapcare.com
VITE_MAP_TILE_URL=https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png
```

## 🤝 **Contributing**

We welcome contributions from the community! Please see our contributing guidelines for:
- Code style and standards
- Pull request process
- Issue reporting
- Feature requests

## 📄 **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 **Contact & Support**

- **Website**: [medimapcare.com](https://medimapcare.com)
- **Email**: contact@medimapcare.com
- **Phone**: +254 700 000 000
- **Support**: Available 24/7 for healthcare emergencies

## 🙏 **Acknowledgments**

- **OpenStreetMap** community for free map data
- **Leaflet.js** team for the mapping library
- **Kenya Health Information System** for healthcare data
- **React** and **Vite** communities for excellent tooling

---

**Built with ❤️ for better healthcare access in Kenya and beyond.**
