# Clini Sync - Bridging Healthcare Professionals and Organizations 🏥🤝


**Seamlessly connect doctors with healthcare organizations, manage patient flow, and streamline medical collaborations through secure digital workflows.**

[![Flutter](https://img.shields.io/badge/Flutter-3.13.9-blue.svg)](https://flutter.dev)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Firebase](https://img.shields.io/badge/Firebase-Emulator%20Ready-orange.svg)](https://firebase.google.com)

## Key Features 🔍

### 🔐 Secure Authentication
- Multi-layer login system (Email+Password & Google Sign-In)
- Role-based access control (Doctor/Organization)
- Aadhar verification for identity validation
- Professional ID verification (Dr. Auth ID/GSTIN)

### 👤 Smart Profile Setup
- Role-specific profile creation
- Unique professional identifiers:
  - Doctors: Custom Authentication ID
  - Organizations: GSTIN Verification
- Secure document storage in Firebase

### 🔗 Intelligent Connection System
- Dual search functionality:
  - Doctors ↔ Organizations via unique IDs
  - QR Code sharing/scanning for instant connections
- Connection request management (Accept/Reject)
- Professional relationship termination controls

### 🕒 Visit Management System
- Customizable visiting schedules:
  - Weekly day selection
  - Time slot configuration
- Real-time schedule synchronization
- Three-state patient tracking:
  - Pending 🕒 | Visited ✅ | Not Visited ❌

### 🚀 Patient Flow Automation
- Organization-side patient registration
- WhatsApp token sharing for appointments
- Doctor-side visit confirmation system
- Cross-platform visit analytics:
  - Daily performance metrics
  - Historical visit patterns

## Tech Stack 💻

**Frontend**  
- Flutter 3.13.9 (Dart 3.1)
- Responsive UI with Material 3 Design
- State Management: Provider + Riverpod

**Backend Services**  
- Firebase Authentication
- Cloud Firestore (NoSQL Database)
- Firebase Storage (Document Verification)

**Key Dependencies**  
- `mobile_scanner`: QR Code operations
- `url_launcher`: WhatsApp integration
- `intl`: Date/time formatting
- `permission_handler`: Device access control

## Getting Started 🚀

### Installation for Users
1. Download latest APK from [Releases Section]
2. Enable "Install from Unknown Sources"
3. Launch and complete secure registration
4. Choose professional role (Doctor/Organization)

### Developer Setup
```bash
git clone https://github.com/yourusername/clini-sync.git
cd clini-sync
flutter pub get
flutter run -d chrome # For web testing
