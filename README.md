# Password Generator App

This is a simple React application that generates random passwords based on user preferences. The app uses various React hooks for state management and side effects.

## Hooks Used

### 1. `useState`

- **Functionality:**
  - `useState` is used to declare and manage state variables in functional components.
  - `length`: Stores the length of the generated password.
  - `numberAllowed`: Stores whether numbers are allowed in the password.
  - `charAllowed`: Stores whether special characters are allowed in the password.
  - `password`: Stores the generated password.

### 2. `useRef`

- **Functionality:**
  - `useRef` is used to create a mutable object that persists throughout the component's lifecycle.
  - `passwordRef`: References the input element for the generated password, enabling interaction with it, such as selecting its text.

### 3. `useCallback`

- **Functionality:**
  - `useCallback` is used to memoize the `generatePassword` function, preventing unnecessary re-creation on each render.
  - The function generates a password based on the specified length and user preferences (numbers and special characters).

### 4. `useEffect`

- **Functionality:**
  - `useEffect` is used to perform side effects in functional components.
  - This hook triggers the `generatePassword` function whenever there are changes to `length`, `numberAllowed`, or `charAllowed.

## Usage

1. Adjust the password length using the range input.
2. Toggle the "Numbers" and "Character" checkboxes to include or exclude them from the password.
3. The generated password is displayed in the input field.
4. Click the "copy" button to copy the password to the clipboard.


