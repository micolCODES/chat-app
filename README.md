# chat-app
A mobile app using React Native. The app allows users to chat, share their location and share pictures (just taken or from the library).

## Key features:
A start Page when the user chooses their chat name and their background
A chat page where the user can chat, share location and images
Data storage on- and offline.

## Technologies used:
JavaScript, React Native, GiftedChat, Firebase, Expo

## Setting up the development environment:
- Initialize the repository on git
- Install Expo CLI as a global npm package: npm install -g expo-cli
- Install all project dependencies:
  1. expo install @react-native-async-storage/async-storage@1.17.3
  2. expo install @react-native-community/netinfo@9.3.0
  3. expo install expo-permissions@13.2.0
  4. expo install expo-image-picker@13.3.1
  5. expo install expo-location@14.3.0
  6. expo install react-native-maps@0.31.1
  7. expo install @expo/react-native-action-sheet@3.14.0
  8. expo install react-navigation@4.4.4
  9. npm install --save-dev @babel/core@7.12.9
- Create a https://expo.dev/ account and log in
- Follow expo CLI's instructions to set up a simulator (XCode, Android Studio, Expo Go)

- **Start the project: expo start**

## Database configuration:
- Go to https://firebase.google.com/ and sign in
- Click on "Create Project"
- Click on "Develop" on the left -> "Cloud Firestore" -> "Create Database": follow the instructions and select "Test Mode"
- Create a new collection called "messages"
- Under "Project Settings", scroll down and click the "Firestore for Web" button (</>)
- Choose a name for the chat app -> click "Register": copy the configuration code to the cloned repository into components/Chat.js
   - replace the following with your configuration code: 
     - apiKey
     - authDomain
     - projectId
     - storageBucket
     - messagingSenderId
     - appId
- To be able to upload photos, go to "Storage" on the left, then the "Rules" tab, then exchange "allow read, write: if false;" for "allow read, write: if true;"

## Main dependencies:
- "@expo/react-native-action-sheet": "3.14.0",
- "@react-native-async-storage/async-storage": "~1.17.3",
- "@react-native-community/masked-view": "^0.1.11",
- "@react-native-community/netinfo": "9.3.0",
- "@react-navigation/bottom-tabs": "^6.4.0",
- "@react-navigation/native": "^6.0.13",
- "@react-navigation/stack": "^6.3.3",
- "expo": "~46.0.16",
- "expo-image-picker": "~13.3.1",
- "expo-location": "~14.3.0",
- "expo-permissions": "~13.2.0",
- "expo-status-bar": "~1.4.0",
- "firebase": "^8.10.1",
- "react": "18.0.0",
- "react-native": "0.69.6",
- "react-native-gesture-handler": "~2.5.0",
- "react-native-gifted-chat": "^1.0.4",
- "react-native-maps": "0.31.1",
- "react-native-reanimated": "^2.12.0",
- "react-native-safe-area-context": "4.3.1",
- "react-native-screens": "~3.15.0",
- "react-navigation": "4.4.4"
