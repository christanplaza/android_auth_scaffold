# Simple Android Login Documentation

Covers the main components of a simple login system.

## 1. LoginActivity

### authenticateUser()

- Logs in the user and redirects to the appropriate activity based on their role (student or parent).

## 2. MainActivity

### logout()

- Logs out the user and redirects back to LoginActivity.

## 3. SessionManager

- Stores and retrieves login state and user role (student or parent).

### setLogin()

- Updates the login state and user role in the app's shared preferences.

### isLoggedIn()

- Returns whether the user is logged in or not.

### getUserRole()

- Returns the user's role (student or parent).

### hasRoleAccess()

- Checks if the user role has access to a specific activity.

## 4. BaseActivity

### checkLoginState()

- Verifies if the user is logged in and has the correct role to access the current activity. If not, redirects to LoginActivity.
