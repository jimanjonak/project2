<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Login Page</title>
</head>
<body style="margin: 0; padding: 0; font-family: Arial, sans-serif; background: linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0.8)), url('./background.jpg') no-repeat center center fixed; background-size: cover; display: flex; justify-content: center; align-items: center; height: 100vh;">
  <div style="width: 100%; max-width: 400px; padding: 30px; background: rgba(255, 255, 255, 0.95); border-radius: 10px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); text-align: center;">
    <img src="./logo.png" alt="Logo" style="width: 70px; margin-bottom: 20px;">
    <h1 style="font-size: 24px; color: #333; margin-bottom: 20px;">User Log In</h1>
    <form>
      <div style="margin-bottom: 15px; text-align: left;">
        <label for="email" style="font-size: 14px; font-weight: bold; color: #555; display: block; margin-bottom: 5px;">Email Address</label>
        <input type="email" id="email" name="email" placeholder="Enter your email" required style="width: 100%; padding: 10px; font-size: 14px; border: 1px solid #ccc; border-radius: 5px;">
      </div>
      <div style="margin-bottom: 15px; text-align: left;">
        <label for="password" style="font-size: 14px; font-weight: bold; color: #555; display: block; margin-bottom: 5px;">Password</label>
        <div style="position: relative;">
          <input type="password" id="password" name="password" placeholder="Enter your password" required style="width: calc(100% - 30px); padding: 10px; font-size: 14px; border: 1px solid #ccc; border-radius: 5px;">
          <span style="position: absolute; right: 10px; top: 50%; transform: translateY(-50%); cursor: pointer; font-size: 16px;" onclick="togglePassword()">👁️</span>
        </div>
      </div>
      <a href="#" style="display: block; font-size: 12px; color: #007BFF; margin: 10px 0; text-decoration: none;">Forgot password?</a>
      <button type="submit" style="width: 100%; padding: 12px; font-size: 16px; background: #005B3F; color: white; border: none; border-radius: 5px; cursor: pointer;">Login</button>
      <p style="margin-top: 10px; font-size: 14px;">Don't have an account? <a href="#" style="color: #007BFF; text-decoration: none;">Sign up</a></p>
    </form>
  </div>

  <script>
    function togglePassword() {
      const passwordField = document.getElementById('password');
      const type = passwordField.type === 'password' ? 'text' : 'password';
      passwordField.type = type;
    }
  </script>
</body>
</html>
