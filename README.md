<!-- index.html -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Girlz Konect</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
  <style>
    body {
      background-color: #ffe6f0;
      text-align: center;
      padding: 50px;
    }
    .btn-custom {
      background-color: #ff66b2;
      border: none;
      font-weight: bold;
      margin: 10px;
      padding: 15px 30px;
      font-size: 20px;
      color: white;
    }
    .cartoon-img {
      opacity: 0.3;
      width: 150px;
      margin: 10px;
      animation: fadeIn 2s ease-in;
    }
    @keyframes fadeIn {
      0% { opacity: 0; }
      100% { opacity: 0.3; }
    }
  </style>
</head>
<body>

  <h1 class="mb-5">Welcome to Girlz Konect</h1>

  <div>
    <img src="https://cdn.pixabay.com/photo/2017/01/31/15/57/avatar-2026510_1280.png" class="cartoon-img">
    <img src="https://cdn.pixabay.com/photo/2017/01/31/20/06/avatar-2027363_1280.png" class="cartoon-img">
  </div>

  <div class="mt-5">
    <a href="register.html" class="btn btn-custom">Register</a>
    <button class="btn btn-custom">Connect to Supplier</button>
    <button class="btn btn-custom">Delete Account</button>
  </div>

</body>
</html>


<!-- register.html -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Register - Girlz Konect</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
  <style>
    body {
      background-color: #ff3385;
      padding: 50px;
      color: white;
    }
    .form-label {
      font-weight: bold;
    }
    .form-control {
      margin-bottom: 20px;
    }
    .form-container {
      max-width: 500px;
      margin: auto;
      padding: 20px;
      background: rgba(255, 255, 255, 0.1);
      border-radius: 10px;
    }
  </style>
</head>
<body>

  <div class="form-container">
    <h2 class="mb-4">Register</h2>
    <div id="success-message" class="alert alert-success d-none" role="alert">
      Registration Successful!
    </div>
    <form id="register-form">
      <div class="mb-3">
        <label for="name" class="form-label">Name</label>
        <input type="text" class="form-control" id="name" required>
      </div>
      <div class="mb-3">
        <label for="age" class="form-label">Age</label>
        <input type="number" class="form-control" id="age" required>
      </div>
      <div class="mb-3">
        <label for="location" class="form-label">Location</label>
        <input type="text" class="form-control" id="location" required>
      </div>
      <div class="mb-3">
        <label for="address" class="form-label">Address (Optional)</label>
        <input type="text" class="form-control" id="address">
      </div>
      <div class="mb-3">
        <label for="contact" class="form-label">Contact Details</label>
        <input type="text" class="form-control" id="contact" required>
      </div>
      <button type="submit" class="btn btn-light">Submit</button>
    </form>
  </div>

<script>
  document.getElementById('register-form').addEventListener('submit', function(event) {
    event.preventDefault();
    document.getElementById('success-message').classList.remove('d-none');
  });
</script>

</body>
</html>
