HTML
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Student Registration Form</title>
  <style>
    body {
      font-family: system-ui, -apple-system, sans-serif;
      background-color: #f4f6f8;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      margin: 0;
    }

    .form-container {
      background-color: #ffffff;
      padding: 2rem;
      border-radius: 8px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
      width: 100%;
      max-width: 400px;
    }

    h1 {
      margin-top: 0;
      margin-bottom: 1.5rem;
      font-size: 1.5rem;
      color: #1f2937;
      text-align: center;
    }

    .form-group {
      margin-bottom: 1.1rem;
    }

    label {
      display: block;
      margin-bottom: 0.4rem;
      font-weight: 600;
      color: #374151;
      font-size: 0.95rem;
    }

    input {
      width: 100%;
      padding: 0.65rem;
      border: 1px solid #d1d5db;
      border-radius: 6px;
      font-size: 1rem;
      box-sizing: border-box;
    }

    input:focus {
      outline: none;
      border-color: #2563eb;
      box-shadow: 0 0 0 3px rgba(37, 99, 235, 0.15);
    }

    button {
      width: 100%;
      padding: 0.75rem;
      background-color: #2563eb;
      color: #ffffff;
      border: none;
      border-radius: 6px;
      font-size: 1rem;
      font-weight: 600;
      cursor: pointer;
      margin-top: 0.5rem;
    }

    button:hover {
      background-color: #1d4ed8;
    }
  </style>
</head>
<body>

  <main class="form-container">
    <h1>Student Registration</h1>
    
    <form action="#" method="post">
      <div class="form-group">
        <label for="full-name">Full Name</label>
        <input 
          type="text" 
          id="full-name" 
          name="full_name" 
          placeholder="Enter your full name" 
          required
        >
      </div>

      <div class="form-group">
        <label for="email">Email</label>
        <input 
          type="email" 
          id="email" 
          name="email" 
          placeholder="student@example.com" 
          required
        >
      </div>

      <div class="form-group">
        <label for="password">Password</label>
        <input 
          type="password" 
          id="password" 
          name="password" 
          placeholder="Create a password" 
          minlength="8" 
          required
        >
      </div>

      <div class="form-group">
        <label for="phone-number">Phone Number</label>
        <input 
          type="tel" 
          id="phone-number" 
          name="phone_number" 
          placeholder="e.g., 9876543210" 
          pattern="[0-9]{10}" 
          title="Please enter a 10-digit phone number" 
          required
        >
      </div>

      <div class="form-group">
        <label for="age">Age</label>
        <input 
          type="number" 
          id="age" 
          name="age" 
          placeholder="Enter your age" 
          min="15" 
          max="100" 
          required
        >
      </div>

      <button type="submit">Register</button>
    </form>
  </main>

</body>
</html>