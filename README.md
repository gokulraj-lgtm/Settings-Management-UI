# Settings Management UI

A modern, fully-featured Settings Management UI built with React, TypeScript, and Tailwind CSS.

## Features

✨ **Modern Design**
- Clean, responsive interface
- Light and dark theme support
- Tailwind CSS styling
- Beautiful icons with Lucide React

🎨 **Customization Options**
- Theme switching (light/dark mode)
- Font size adjustment (small, medium, large)
- Language selection (English, Spanish, French)
- Privacy level settings

🔔 **Notification Management**
- Push notifications toggle
- Email notifications toggle
- Granular control over notification preferences

🔒 **Security & Privacy**
- Two-factor authentication toggle
- Privacy level selection (public/private)
- Secure settings management

💾 **Persistence**
- Local storage integration
- Automatic settings saving
- Settings restoration on page reload

⚡ **Performance**
- Built with Vite for fast development
- Optimized TypeScript configuration
- Responsive and smooth UI interactions

## Technology Stack

- **React 18** - UI framework
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Utility-first CSS framework
- **Vite** - Fast build tool and dev server
- **Lucide React** - Beautiful icon library

## Getting Started

### Prerequisites
- Node.js 16+ and npm

### Installation

```bash
# Navigate to project directory
cd "Settings Management UI"

# Install dependencies
npm install
```

### Development

```bash
# Start the development server
npm run dev
```

The application will automatically open at `http://localhost:5173`

### Build

```bash
# Build for production
npm run build

# Preview production build
npm run preview
```

## Project Structure

```
Settings Management UI/
├── src/
│   ├── components/
│   │   ├── AppearanceSettings.tsx
│   │   ├── NotificationsSettings.tsx
│   │   ├── SecuritySettings.tsx
│   │   └── SettingsActions.tsx
│   ├── hooks/
│   │   └── useSettings.ts
│   ├── App.tsx
│   ├── main.tsx
│   └── index.css
├── public/
├── index.html
├── package.json
├── vite.config.ts
├── tsconfig.json
├── tailwind.config.js
└── postcss.config.js
```

## Settings Structure

The application manages the following settings:

```typescript
interface Settings {
  theme: 'light' | 'dark';
  notifications: boolean;
  emailNotifications: boolean;
  autoSave: boolean;
  language: 'en' | 'es' | 'fr';
  fontSize: 'small' | 'medium' | 'large';
  privacy: 'public' | 'private';
  twoFactor: boolean;
}
```

## Key Components

### `useSettings` Hook
Custom React hook that manages settings state and localStorage persistence.

### `AppearanceSettings`
Component for managing theme, font size, and language preferences.

### `NotificationsSettings`
Component for managing push and email notification preferences.

### `SecuritySettings`
Component for managing privacy levels and two-factor authentication.

### `SettingsActions`
Component with save and reset buttons for settings management.

## Usage

The application automatically persists all settings to the browser's localStorage. Changes are saved immediately when toggling options.

### Theme Management
- Switch between light and dark themes with a single click
- Theme preference is saved and restored on page reload

### Notifications
- Toggle push notifications independently from email notifications
- Settings are applied immediately

### Security Options
- Choose between public and private privacy levels
- Enable two-factor authentication for added security

## Browser Support

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+

## Contributing

Feel free to extend this project with additional settings categories or features!

## License

MIT
