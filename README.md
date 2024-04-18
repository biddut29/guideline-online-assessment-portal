# guideline-online-assessment-portal

1. Clone the branch
2. Open the terminal and execute the following commands:
   ```
   npm install
   npm run build
   ```
3. Copy the listed files and folders to a designated location:
   - package.json
   - .env
   - .next
   - public
   - package-lock.json
   - (You can create the node_modules folder later by running `npm install`)

4. Navigate to the designated location and open the .env file. Update the Firebase configuration with the credentials obtained from your Firebase project settings:
   - Navigate to your Firebase project settings [here](https://console.firebase.google.com/).
   - Go to Project Overview -> Project Settings -> Your apps.
   Update the following Firebase configurations in the .env file:
   ```
   # FIREBASE
   NEXT_PUBLIC_FIREBASE_API_KEY=Your_API_Key
   NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=Your_Auth_Domain
   NEXT_PUBLIC_FIREBASE_PROJECT_ID=Your_Project_ID
   NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=Your_Storage_Bucket
   NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=Your_Messaging_Sender_ID
   NEXT_PUBLIC_FIREBASE_APPID=Your_App_ID
   NEXT_PUBLIC_FIREBASE_MEASUREMENT_ID=Your_Measurement_ID
   ```

![image](https://github.com/biddut29/guideline-online-assessment-portal/assets/112966490/245e8a1e-fe95-408d-950b-1e71820c5cbc)

   

5. Update the Google ID and secret for SSO (Single Sign-On) using the credentials obtained from Google SSO configuration:
   - Navigate to your Google API credentials [here](https://console.cloud.google.com/apis/credentials).
   - Obtain the Client ID for the Web application.
   Update the following configurations in the .env file:
   ```
   GOOGLE_ID=Your_Google_Client_ID
   GOOGLE_SECRET=Your_Google_Client_Secret
   ADMIN_BASIC_CREDENTIALS=Your_Admin_Basic_Credentials
   ```
6. You can change the admin credentails
   Update the following configurations in the .env file:
   ``` 
   ADMIN_BASIC_CREDENTIALS=Your_Admin_Basic_Credentials
   ```   

7. Open the terminal and ensure that Node.js version is >= v18.17.0. Then run the following commands:
   ```
   npm install
   npm run start
   ```

These steps should set up and configure your project correctly.
