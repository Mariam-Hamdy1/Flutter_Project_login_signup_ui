# Flutter Login & Sign Up Screen UI

This Flutter project is a simple and clean implementation of **Login** and **Sign Up** screens. It demonstrates how to design a user interface with navigation between two authentication screens, including input fields and styled buttons, using only Flutter's built-in widgets.

---

## 🧠 Project Explanation

### 📱 Purpose

This app serves as a UI prototype for a typical authentication flow found in many mobile apps. It does **not** include real backend functionality (like Firebase), but the structure is ready to integrate real authentication logic later.

---

### 🧱 Structure & How It Works

#### 1. `main.dart`

- This is the entry point of the app.
- It runs the `MyApp` widget which uses `MaterialApp` to set up the app's theme and home screen.
- The home screen is set to the `LoginScreen`.

```dart
home: const LoginScreen(),
2. login_screen.dart
Displays the Login screen UI:

A welcome message

TextField for username and password

A "Login" button

A "Forgot Password" link

A prompt: "Don't have an account? Sign Up"

The Sign Up link uses Navigator.push() to take the user to the SignUpScreen.

dart
Copy
Edit
Navigator.push(
  context,
  MaterialPageRoute(builder: (context) => const SignUpScreen()),
);
3. signup_screen.dart
Displays the Sign Up screen UI:

Fields for username, email, password, and confirm password

A "Sign Up" button

A divider with an "Or" option

A "Sign In with Google" placeholder

A prompt: "Already have an account? Login"

The Login link takes the user back to the LoginScreen using the same navigation approach.

🎨 UI Components Used
TextField for input

ElevatedButton for primary actions

Icon, IconButton for icons and interactions

GestureDetector to handle text tap events

Navigator.push for screen navigation

SingleChildScrollView on Sign Up screen to make it scrollable on small screens

💡 Why This Project is Useful
Teaches the basic structure of Flutter apps

Shows how to navigate between screens

Provides a foundation for adding authentication logic

Demonstrates clean layout and responsive design principles

🔄 Future Enhancements
Add form validation

Integrate Firebase Authentication

Use Provider or Riverpod for state management

Add password visibility toggle

Add loading indicators and error handling

📸 Preview
<img width="725" height="1023" alt="LoginScreen" src="https://github.com/user-attachments/assets/e3652ec6-218d-45ef-b59b-99fa1794b930" />
<img width="697" height="1022" alt="SignupScreen" src="https://github.com/user-attachments/assets/08490770-3c6d-4175-9cd9-ad4c1ffd6f76" />
