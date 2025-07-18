# MyShop For Hackers!

Welcome to MyShop! This is a simple e-commerce app with a React frontend and Node.js/Express backend. Follow these steps to run the project locally.

---

## 1. Download and unzip the project
- Download the zip file from GitHub.
- Unzip it to your desired location (e.g., `E:/Folder/MyShop`).
- Open the unzipped folder in VS Code or your editor.

## 2. Install dependencies
```sh
cd server
npm install
npm install express mongoose mongodb cors dotenv bcryptjs jsonwebtoken nodemailer nodemon
```
```sh
cd ../client
npm install
npm install react react-dom react-router-dom axios react-icons react-scripts @testing-library/react @testing-library/jest-dom @testing-library/user-event @testing-library/dom web-vitals
```

## 3. Set up environment variables
- Go to `server/.env` and add your own values for:
  - `MONGO_URI` (your MongoDB connection string)
  - `JWT_SECRET` (any random string)
  - `MAIL_USER`, `MAIL_PASS`, `ADMIN_EMAIL` (for email notifications, use Gmail and an app password)

## 4. Start the backend
```sh
cd server
npm start
```
- The backend runs on [http://localhost:5000](http://localhost:5000)

## 5. Start the frontend
```sh
cd client
npm start
```
- The frontend runs on [http://localhost:3000](http://localhost:3000)

## 6. Login & Admin
- Register a user, then set their role to `admin` in the database to access the admin dashboard. Like , in your mongoDB , the rold of isAdmin will be false, make them admin , whom you want to.
- Admins can add/edit/delete products and view orders , but login using that admin account to access the admin dashboard.

## 7. Email setup
- For order notifications, set up Gmail and use an app password (Google account > Security > App passwords). using app password is important , it looks like "xyzx abcd abcd ubfg" something like this. Don't use your normal Gmail's password, it wont work.

---

## Troubleshooting
- If you see errors, check your `.env` values and make sure MongoDB is running.
- For email issues, double-check your Gmail/app password setup.

---

## Have fun!
If you get stuck, just ask for help - Instagram: gh0st_cipher. Enjoy hacking on MyShop!
