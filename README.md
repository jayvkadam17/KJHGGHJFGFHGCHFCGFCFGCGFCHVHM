<!DOCTYPE html>
<html>
<head>
  <title>User Info and Login System</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <div class="container">
    <div class="form-container" id="signup-container">
      <h1>Sign Up</h1>
      <form id="signup-form">
        <input type="text" placeholder="Name" id="name" required>
        <input type="text" placeholder="Username" id="username" required>
        <input type="text" placeholder="Bio" id="bio" required>
        <input type="email" placeholder="Email" id="email" required>
        <input type="password" placeholder="Password" id="password" required>
        <button type="submit">Sign Up</button>
        <p>Already have an account? <a href="#" id="login-link">Login</a></p>
      </form>
    </div>
    <div class="form-container" id="login-container">
      <h1>Login</h1>
      <form id="login-form">
        <input type="text" placeholder="Username" id="login-username" required>
        <input type="password" placeholder="Password" id="login-password" required>
        <button type="submit">Login</button>
        <p>Don't have an account? <a href="#" id="signup-link">Sign Up</a></p>
      </form>
    </div>
    <div class="user-page" id="user-page" style="display: none;">
      <h1>Welcome to User Page</h1>
      <img src="demo-image.jpg" alt="User Demo Image">
      <div class="user-data" id="user-data">
        <!-- User data will be fetched and displayed here -->
      </div>
      <button id="logout-button">Logout</button>
    </div>
  </div>
  <script src="script.js"></script>
</body>
</html
  /////////////////////////////////////////////////////////////
  body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.form-container, .user-page {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  border: 1px solid #ccc;
  padding: 20px;
  width: 300px;
}

.user-page {
  display: none;
}

input[type="text"], input[type="email"], input[type="password"] {
  padding: 10px;
  margin-bottom: 10px;
  width: 100%;
}

button {
  padding: 10px;
  width: 100%;
  background-color: #007BFF;
  color: #fff;
  border: none;
  cursor: pointer;
}

p {
  margin: 10px 0;
}

a {
  color: #007BFF;
  text-decoration: none;
}

body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.form-container, .user-page {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  border: 1px solid #ccc;
  padding: 20px;
  width: 300px;
}

.user-page {
  display: none;
}

input[type="text"], input[type="email"], input[type="password"] {
  padding: 10px;
  margin-bottom: 10px;
  width: 100%;
}

button {
  padding: 10px;
  width: 100%;
  background-color: #007BFF;
  color: #fff;
  border: none;
  cursor: pointer;
}

p {
  margin: 10px 0;
}

a {
  color: #007BFF;
  text-decoration: none;
}

body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.form-container, .user-page {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  border: 1px solid #ccc;
  padding: 20px;
  width: 300px;
}

.user-page {
  display: none;
}

input[type="text"], input[type="email"], input[type="password"] {
  padding: 10px;
  margin-bottom: 10px;
  width: 100%;
}

button {
  padding: 10px;
  width: 100%;
  background-color: #007BFF;
  color: #fff;
  border: none;
  cursor: pointer;
}

p {
  margin: 10px 0;
}

a {
  color: #007BFF;
  text-decoration: none;
}

body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.form-container, .user-page {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  border: 1px solid #ccc;
  padding: 20px;
  width: 300px;
}

.user-page {
  display: none;
}

input[type="text"], input[type="email"], input[type="password"] {
  padding: 10px;
  margin-bottom: 10px;
  width: 100%;
}

button {
  padding: 10px;
  width: 100%;
  background-color: #007BFF;
  color: #fff;
  border: none;
  cursor: pointer;
}

p {
  margin: 10px 0;
}

a {
  color: #007BFF;
  text-decoration: none;
}

body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.form-container, .user-page {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  border: 1px solid #ccc;
  padding: 20px;
  width: 300px;
}

.user-page {
  display: none;
}

input[type="text"], input[type="email"], input[type="password"] {
  padding: 10px;
  margin-bottom: 10px;
  width: 100%;
}

button {
  padding: 10px;
  width: 100%;
  background-color: #007BFF;
  color: #fff;
  border: none;
  cursor: pointer;
}

p {
  margin: 10px 0;
}

a {
  color: #007BFF;
  text-decoration: none;
}

////////////////////////////////////////////////////
const signupContainer = document.getElementById('signup-container');
const loginContainer = document.getElementById('login-container');
const userPage = document.getElementById('user-page');
const signupForm = document.getElementById('signup-form');
const loginForm = document.getElementById('login-form');
const userData = document.getElementById('user-data');
const logoutButton = document.getElementById('logout-button');
const loginLink = document.getElementById('login-link');
const signupLink = document.getElementById('signup-link');

signupForm.addEventListener('submit', (e) => {
  e.preventDefault();
  const name = document.getElementById('name').value;
  const username = document.getElementById('username').value;
  const bio = document.getElementById('bio').value;
  const email = document.getElementById('email').value;
  const password = document.getElementById('password').value;

  // Implement signup API request here using fetch or axios
  // After successful signup, show the login page
  // Redirect user to login page
  loginContainer.style.display = 'flex';
  signupContainer.style.display = 'none';
});

loginForm.addEventListener('submit', (e) => {
  e.preventDefault();
  const username = document.getElementById('login-username').value;
  const password = document.getElementById('login-password').value;

  // Implement login API request here using fetch or axios
  // After successful login, show the user page
  // Redirect user to user page
  userPage.style.display = 'flex';
  loginContainer.style.display = 'none';
});

logoutButton.addEventListener('click', () => {
  // Implement logout API request here using fetch or axios
  // After successful logout, show the login page again
  // Redirect user to login page
  loginContainer.style.display = 'flex';
  userPage.style.display = 'none';
});

loginLink.addEventListener('click', (e) => {
  e.preventDefault();
  loginContainer.style.display = 'flex';
  signupContainer.style.display = 'none';
});

signupLink.addEventListener('click', (e) => {
  e.preventDefault();
  signupContainer.style.display = 'flex';
  loginContainer.style.display = 'none';
});

// Fetch user data and display it on the user page
// You can use the authenticated JWT token in the headers to fetch user data from the backend API
// Use fetch or axios to make the API request

// Example:
// const token = '
//////////////////////////////////////////////////
const signupContainer = document.getElementById('signup-container');
const loginContainer = document.getElementById('login-container');
const userPage = document.getElementById('user-page');
const signupForm = document.getElementById('signup-form');
const loginForm = document.getElementById('login-form');
const userData = document.getElementById('user-data');
const logoutButton = document.getElementById('logout-button');
const loginLink = document.getElementById('login-link');
const signupLink = document.getElementById('signup-link');

signupForm.addEventListener('submit', (e) => {
  e.preventDefault();
  const name = document.getElementById('name').value;
  const username = document.getElementById('username').value;
  const bio = document.getElementById('bio').value;
  const email = document.getElementById('email').value;
  const password = document.getElementById('password').value;

  // Implement signup API request here using fetch or axios
  // After successful signup, show the login page
  // Redirect user to login page
  loginContainer.style.display = 'flex';
  signupContainer.style.display = 'none';
});

loginForm.addEventListener('submit', (e) => {
  e.preventDefault();
  const username = document.getElementById('login-username').value;
  const password = document.getElementById('login-password').value;

  // Implement login API request here using fetch or axios
  // After successful login, show the user page
  // Redirect user to user page
  userPage.style.display = 'flex';
  loginContainer.style.display = 'none';
});

logoutButton.addEventListener('click', () => {
  // Implement logout API request here using fetch or axios
  // After successful logout, show the login page again
  // Redirect user to login page
  loginContainer.style.display = 'flex';
  userPage.style.display = 'none';
});

loginLink.addEventListener('click', (e) => {
  e.preventDefault();
  loginContainer.style.display = 'flex';
  signupContainer.style.display = 'none';
});

signupLink.addEventListener('click', (e) => {
  e.preventDefault();
  signupContainer.style.display = 'flex';
  loginContainer.style.display = 'none';
});

// Fetch user data and display it on the user page
// You can use the authenticated JWT token in the headers to fetch user data from the backend API
// Use fetch or axios to make the API request

// Example:
// const token = '

