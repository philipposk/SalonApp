Here’s your full edited version with **Emily → SalonApp** and all references to nails replaced with **general beauty/wellness services**:

---

The SalonApp - 

A comprehensive iOS application built with SwiftUI for managing beauty salons and studios, providing a complete ecosystem for clients, technicians, and administrators.

## 📱 Overview

SalonApp is a full-featured beauty and wellness management system that combines client booking, e-commerce, professional tools, and business analytics into a single, beautifully designed iOS app. The app supports multiple user roles, customizable UI themes, and real-time features powered by Supabase.

## ✨ Key Features

### 🎯 Client Features

* **Online Booking System** - Calendar and list views with 60-day booking window
* **Service Menu** - Browse services with pricing, duration, and descriptions
* **Technician Portfolios** - View artist profiles, expertise, and work galleries
* **Product Shop** - Purchase beauty products, supplies, and salon essentials
* **Reward & Loyalty System** - Earn points for bookings and redeem rewards
* **Waitlist** - Join waitlists for preferred time slots
* **Photo Upload** - Guided photo capture for face, hair, nails, and full body
* **Multiple UI Themes** - Beauty Card, Feed, Sidebar, and Modern layouts
* **Dark/Light Mode** - System-aware theme customization
* **AI Chatbot** - Interactive assistant with multiple personality modes

### 👨‍💼 Professional/Technician Features

* **Schedule Management** - View and manage appointments
* **Portfolio Management** - Upload and showcase work
* **Earnings Projection** - Track commissions and earnings
* **Statistics Dashboard** - View performance metrics
* **Availability Management** - Set working hours and unavailable dates
* **Real-time Chat** - Private and group messaging with admins
* **Client History** - Access client booking history and preferences

### 👑 Admin Features

* **Complete Dashboard** - Overview of bookings, revenue, and operations
* **Personnel Management** - Approve technicians, admins, and staff
* **Service Management** - Add, edit, and configure services
* **Finance Hub** - Payroll management, cashflow coach, and financial analytics
* **AI Search** - Intelligent keyword and advanced search across the system
* **Notification System** - Service/artist mismatch alerts and admin notifications
* **Statistics & Analytics** - Comprehensive business insights
* **Theme Customization** - Create and manage custom UI themes
* **Widget Management** - Configure dashboard widgets for different roles
* **Mass Appointment Insertion** - Bulk import appointments via OCR/document parsing
* **Demo Mode** - Simulate appointments for testing

### 💰 Finance Module

* **Payroll Management** - Hourly, commission, hybrid compensation models
* **Cashflow Coach** - AI-powered 30-day cashflow forecasting
* **Payment Settings** - Stripe, PayPal, bank transfer integration
* **Expense Tracking** - Monitor salon expenses
* **Revenue Analytics** - Track income and projections

### 💬 Communication

* **Real-time Chat** - Private and group messaging for staff
* **AI Chatbot** - Multiple personality modes (Daisy, Granny, Karen, Max, etc.)
* **Push Notifications** - Appointment reminders, promotions, and updates
* **Email Integration** - Automated email notifications

### 🎨 Customization

* **Multiple UI Layouts** - Beauty Card, Feed, Sidebar, Modern, Floating Panel
* **Theme System** - Custom colors, fonts, and styling
* **Logo Management** - Theme-specific logo customization
* **Translation Support** - English and Greek (extensible to more languages)
* **Currency Support** - Multi-currency support with EUR default

## 🏗️ Architecture

### Tech Stack

* **Language**: Swift 5.9+
* **UI Framework**: SwiftUI
* **Backend**: Supabase (PostgreSQL, Realtime, Storage, Auth)
* **Authentication**: Email, Google OAuth, Facebook OAuth
* **AI Integration**: OpenAI API (configurable)
* **Storage**: Hybrid (Supabase + UserDefaults for caching)

### Key Components

* **AuthenticationManager** - Handles user authentication and OAuth
* **BookingManager** - Manages appointments and availability
* **ProductManager** - E-commerce product management
* **ChatManager** - Real-time messaging system
* **ChatbotManager** - AI chatbot integration
* **FinanceCloudService** - Financial data synchronization
* **ThemeManager** - Theme and UI customization
* **PermissionManager** - Role-based access control

## 👥 User Roles

The app supports multiple user roles with different permissions:

* **Guest** - Limited access, can browse and book
* **User/Member** - Full client features
* **Technician/Professional** - Artist tools and schedule management
* **Admin** - Full system access
* **Manager** - Administrative access with limited permissions
* **Front Desk** - Reception and booking management
* **Finance** - Financial data access
* **Marketing** - Promotional content management
* **Support** - Customer support tools
* **Supplier** - Product supplier access

## 🚀 Getting Started

### Prerequisites

* Xcode 15.0 or later
* iOS 17.0+ deployment target
* Swift 5.9+
* Supabase account (free tier works)

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/salonapp.git
   cd salonapp
   ```

2. **Set up Supabase**

   * Follow the [Supabase Setup Guide](SETUP_SUPABASE.md)
   * Create a Supabase project
   * Get your project URL and anon key
   * Configure authentication providers (Email, Google, Facebook)

3. **Configure the App**

   * Open `apapp.xcodeproj` in Xcode
   * Update `AuthenticationManager.swift` with your Supabase credentials
   * Configure OpenAI API key in Settings (admin-only)

4. **Run the App**

   * Select your target device or simulator
   * Build and run (⌘R)

### Initial Setup

1. **First Launch**

   * Sign up or sign in with email/social login
   * Complete the app introduction
   * Choose your preferred UI layout

2. **Admin Setup**

   * First user automatically becomes admin
   * Configure business information in Admin → Salon Settings
   * Add services, technicians, and products
   * Set up payment methods

3. **Configure Services**

   * Go to Admin → Service Management
   * Add services with pricing and duration
   * Configure booking rules, categories, and availability

## 📚 Documentation

* [Supabase Setup Guide](SETUP_SUPABASE.md)
* [Chat Setup Guide](CHAT_SETUP.md)
* [Finance Module Specification](FINANCE_MODULE_SPEC.md)
* [Guided Photo Capture](GUIDED_PHOTO_CAPTURE.md)
* [Implementation Status](IMPLEMENTATION_STATUS.md)
* [App Enhancement Recommendations](APP_ENHANCEMENT_RECOMMENDATIONS.md)

## 🎯 Roadmap

### Completed ✅

* Online booking system with multiple UI layouts
* Service and product management
* Reward/loyalty system
* Real-time chat for staff
* AI chatbot with multiple personalities
* Finance module (payroll, cashflow coach)
* Admin dashboard and analytics
* Theme customization system
* Photo upload with guided capture
* Multi-currency support

### In Progress 🔄

* Widget editing for all roles
* Enhanced booking confirmed messages
* Logo system improvements
* Better terminology throughout app

### Planned 📋

* Gift cards system
* Package deals and promotions
* Blog/inspiration section
* Membership subscriptions
* In-app client reviews
* Forms and waivers
* Referral program
* Multiple locations support

## 🔒 Security

* **API Keys**: No hardcoded keys - configured by admin in settings
* **Authentication**: Secure OAuth and email authentication via Supabase
* **Data Privacy**: Row Level Security (RLS) policies in Supabase
* **User Data**: Encrypted storage with proper access controls

## 🌍 Localization

Currently supports:

* English (en)
* Greek (el)

The translation system is extensible - add more languages via `TranslationManager`.

## 📱 Requirements

* **iOS**: 17.0 or later
* **Devices**: iPhone (iPad support coming soon)
* **Xcode**: 15.0 or later
* **Swift**: 5.9+

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👤 Author

**Philippos Dimitrios Ktistakis**

## 🙏 Acknowledgments

* Built with [SwiftUI](https://developer.apple.com/xcode/swiftui/)
* Backend powered by [Supabase](https://supabase.com)
* AI features powered by [OpenAI](https://openai.com)

## 📞 Support

For support, email [phktistakis@gmail.com](phktistakis@gmail.com) or open an issue in this repository.

---

**Made with ❤️ for beauty professionals everywhere**

---
