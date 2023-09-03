<!DOCTYPE html>
<html>
<div>
  <button onclick="showLogin()">Log In</button>
  <button onclick="showSignUp()">Sign Up</button>
</div>

<div id="loginForm" style="display: none;">
  <form>
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>
  
    <label for="password">Password:</label>
    <input type="password" id="password" name="password" required>

    <input type="submit" value="Log In">
  </form>
</div>

<div id="signupForm" style="display: none;">
  <form>
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>
  
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>
  
    <label for="password">Password:</label>
    <input type="password" id="password" name="password" required>

    <input type="submit" value="Sign Up">
  </form>
</div>

<script>
  function showLogin() {
    document.getElementById("loginForm").style.display = "block";
    document.getElementById("signupForm").style.display = "none";
  }

  function showSignUp() {
    document.getElementById("loginForm").style.display = "none";
    document.getElementById("signupForm").style.display = "block";
  }
</script>

<style>
    /* Center the image */
    .center {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    /* Set the image size */
    .image {
      max-width: 100%;
      max-height: 100%;
    }
  </style>
<body>
  <div class="center">
    <img class="image" src="" alt="Your Image">
  </div>
</body>
</html>
