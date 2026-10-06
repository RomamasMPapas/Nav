# Nav

## Royette Andrei C. Telar

## Preview

<div align="center">
  <img src="demo.gif" width="300" alt="Preview" /><br><br>
  <a href="demo.mp4">Open demo.mp4</a>
</div>

## Features

- Login screen with mocked email and password flow
- Drawer navigation for app sections
- Bottom tab navigation for main screens
- Dashboard overview with quick metrics cards
- Contacts list with avatar-based contact cards
- Contact detail screen with action buttons and profile information
- Profile and settings screen with user account details and logout action
- Material 3 styling inspired by Google design patterns

## Tech Stack

- Flutter
- Dart
- Material 3 UI
- Google Nav Bar package
- Custom theme and color palette based on Google colors

## Project Structure

```text
lib/
├── core/
│   └── theme/
│       └── google_colors.dart
├── data/
│   └── repositories/
│       └── contact_repository.dart
├── domain/
│   └── models/
│       ├── contact.dart
│       └── user.dart
├── presentation/
│   ├── auth/
│   │   └── login_screen.dart
│   ├── contacts/
│   │   ├── contact_detail_screen.dart
│   │   └── contacts_list_tab.dart
│   ├── dashboard/
│   │   └── dashboard_tab.dart
│   ├── main_nav/
│   │   └── main_navigation_screen.dart
│   └── profile/
│       └── profile_settings_tab.dart
├── main.dart
└── ...
```

## Screen Descriptions

### Login Screen
- Entry point of the app
- Accepts email and password input
- Uses mocked user data for demo navigation
- Redirects the user to the main navigation flow after sign in

### Dashboard
- Displays a welcome card for the authenticated user
- Shows quick overview metrics such as contacts count, favorites, storage, and security status
- Includes a button to navigate directly to the contacts list

### Contacts List
- Renders a searchable-style list of contact cards using a repository
- Each item includes an avatar, name, and email
- Tapping a contact opens the detail view

### Contact Detail Screen
- Shows the selected contact's avatar, name, role, and contact information
- Contains action buttons for call, text, and email
- Displays phone number and email in a clean card layout

### Profile & Settings
- Shows account information and role
- Includes settings-style list tiles for notifications, security, and app theme
- Provides logout action to return to the login screen

### Main Navigation
- Handles the drawer navigation and bottom tab bar
- Keeps track of the selected tab and swaps the active screen content
- Includes a logout action that restores the login screen
