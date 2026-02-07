<div align="center">

# Wandora - Travel & Tour Platform

[![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)](https://vitejs.dev/)
[![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)](https://vercel.com/)

[Live Demo](https://wandora.vercel.app) • [Backend Repo](https://github.com/zahid-official/project-01-wandora-backend) • [Report Bug](https://github.com/zahid-official/project-01-wandora/issues)

</div>

---

## 📖 Overview

Wandora is a modern travel and tour booking platform that offers seamless tour discovery, booking management, and user-friendly interfaces. Built with React and TypeScript, it delivers a fast, responsive experience for travelers looking to explore and book their next adventure.

---

## ⚡ Tech Stack

| Category | Technology |
|----------|-----------|
| **Framework** | React 18 + TypeScript |
| **Build Tool** | Vite |
| **Styling** | TailwindCSS + DaisyUI |
| **State Management** | React Context / Redux |
| **Routing** | React Router v6 |
| **Forms** | React Hook Form + Zod |
| **HTTP Client** | Axios |
| **Animations** | Framer Motion |
| **Icons** | React Icons |
| **Package Manager** | pnpm |

---

## ✨ Key Features

### 🎯 Tour Discovery
- Advanced search and filtering
- Category-based browsing
- Featured tour highlights
- Detailed tour information with galleries
- Real-time availability tracking

### 🎫 Booking Management
- Intuitive booking flow
- Date and group size selection
- Instant booking confirmation
- Booking history and tracking
- Cancellation handling

### 👤 User Experience
- Secure authentication (Login/Register)
- Personal profile management
- Responsive design (mobile-first)
- Fast page loads with Vite
- Smooth animations and transitions

### 💳 Payment Integration
- Secure payment processing
- Multiple payment methods
- Transaction history
- Email confirmations

### 🔐 Security
- JWT-based authentication
- Protected routes
- Form validation
- XSS protection

---

## 📁 Project Structure

```
src/
├── components/
│   ├── common/          # Reusable UI components
│   │   ├── Button.tsx
│   │   ├── Card.tsx
│   │   ├── Modal.tsx
│   │   └── Spinner.tsx
│   ├── layout/          # Layout components
│   │   ├── Header.tsx
│   │   ├── Footer.tsx
│   │   └── Navbar.tsx
│   └── features/        # Feature-specific components
│       ├── tours/
│       ├── booking/
│       └── auth/
│
├── pages/
│   ├── Home.tsx
│   ├── Tours.tsx
│   ├── TourDetails.tsx
│   ├── Booking.tsx
│   ├── Profile.tsx
│   ├── Login.tsx
│   └── Register.tsx
│
├── hooks/               # Custom React hooks
│   ├── useAuth.ts
│   ├── useTours.ts
│   └── useBooking.ts
│
├── context/             # React Context
│   ├── AuthContext.tsx
│   └── BookingContext.tsx
│
├── services/            # API services
│   ├── api.ts
│   ├── authService.ts
│   ├── tourService.ts
│   └── bookingService.ts
│
├── utils/               # Utility functions
│   ├── validation.ts
│   ├── formatters.ts
│   └── constants.ts
│
├── types/               # TypeScript types
│   └── index.ts
│
├── routes/              # Route configuration
│   └── AppRoutes.tsx
│
└── App.tsx              # Main app component
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ 
- pnpm (recommended) or npm

### Installation

```bash
# Clone the repository
git clone https://github.com/zahid-official/project-01-wandora.git
cd project-01-wandora

# Install dependencies
pnpm install

# Set up environment variables
cp .env.example .env
```

### Environment Variables

```env
VITE_API_URL=http://localhost:5000/api
VITE_APP_NAME=Wandora
VITE_PAYMENT_PUBLIC_KEY=your_payment_key
```

### Development

```bash
# Start development server
pnpm dev

# Build for production
pnpm build

# Preview production build
pnpm preview

# Run linter
pnpm lint
```

The app will be available at `http://localhost:5173`

---

## 🎨 UI Components

Built with **TailwindCSS** and **DaisyUI** for consistent, accessible design:

- Custom button variants
- Responsive cards
- Modal dialogs
- Form inputs with validation
- Loading states
- Toast notifications
- Image galleries

---

## 🔌 API Integration

All API calls are handled through centralized services:

```typescript
// Example: Fetching tours
import { tourService } from '@/services/tourService';

const tours = await tourService.getAllTours({
  category: 'adventure',
  destination: 'Nepal',
  maxPrice: 2000
});
```

---

## 🛡️ Protected Routes

```typescript
<Route element={<ProtectedRoute />}>
  <Route path="/profile" element={<Profile />} />
  <Route path="/bookings" element={<MyBookings />} />
  <Route path="/booking/:tourId" element={<Booking />} />
</Route>
```

---

## 📱 Responsive Design

- **Mobile-first** approach
- Breakpoints: `sm`, `md`, `lg`, `xl`, `2xl`
- Touch-friendly interfaces
- Optimized images for all devices

---

## ⚙️ Build & Deployment

### Production Build
```bash
pnpm build
```

### Deploy to Vercel
```bash
vercel --prod
```

The project is configured for automatic deployment on Vercel with optimized build settings.

---

## 🧪 Code Quality

```bash
# Type checking
pnpm tsc --noEmit

# Linting
pnpm lint

# Format code
pnpm format
```

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License.

---

## 🌟 Author

<div align="center">
  <a href="https://github.com/zahid-official">
    <img src="https://github.com/zahid-official.png" width="100" height="100" style="border-radius: 50%;" alt="Zahid Official" />
  </a>
  
  <h3>Zahid Official</h3>
  <p><i>Full Stack Developer | React Enthusiast</i></p>
  
  [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/zahid-official)
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/zahid-web)
  [![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:zahid.official8@gmail.com)
  
  <p><i>Crafting delightful web experiences with modern technologies</i></p>
</div>

---

<div align="center">
  <p>If you found this project helpful, please consider giving it a ⭐</p>
</div>
