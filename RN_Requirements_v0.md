### **Feature Overview**
Implement a Google Sign-In screen for a React Native app. Only users with authorized email addresses will be allowed access to the app. Unauthorized users will see an error message and will not proceed further.

---

### **Requirements**

#### **UI Requirements**
1. Create a single screen with:
   - A title: "Login with Google".
   - A button labeled "Sign in with Google".
   - A placeholder for error messages (e.g., a `Text` component below the button).

2. The UI should be simple and functional, with no additional styling beyond basic alignment.

---

#### **Logic Requirements**
1. Use the `@react-native-google-signin/google-signin` library for Google authentication.
2. Maintain a list of authorized email addresses in the code (example list below):
   ```javascript
   const authorizedEmails = [
     "authorized_user1@example.com",
     "authorized_user2@example.com",
     "authorized_user3@example.com"
   ];
   ```

3. After the user signs in:
   - Check if the signed-in user's email is in the `authorizedEmails` list.
   - If authorized:
     - Print a success message to the console (e.g., "Access granted to [email]").
     - Navigate to the next screen (placeholder for future implementation).
   - If unauthorized:
     - Display an error message below the "Sign in with Google" button (e.g., "Access denied. Your email is not authorized.").

---

#### **Firebase Configuration**
1. Set up Firebase for the app:
   - Add the `google-services.json` file to the `android/app` directory.
   - Add the `GoogleService-Info.plist` file to the `ios` directory.
   - Enable Google Sign-In in the Firebase Console under "Authentication".

---

#### **Code Structure**
1. Create a `LoginScreen` component.
2. Use the `GoogleSignin` class to handle authentication.
3. Implement the logic for checking authorized emails and displaying error messages.

---

### Example Authorized Email List
Replace the example email list in the code with the real list of authorized emails:
- `elaine.batista1105@gmail.com`
- `paulamcunha31@gmail.com`
- `edbpmc@gmail.com`