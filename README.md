<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>College Admission Form</title>
<style>
  body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    margin: 0;
    padding: 0;
  }
  .form-container {
    max-width: 700px;
    margin: 50px auto;
    padding: 20px;
    background-color: #fff;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
  h2 {
    text-align: center;
    margin-bottom: 20px;
  }
  .input-group {
    margin-bottom: 15px;
  }
  .input-group label {
    display: block;
    margin-bottom: 5px;
  }
  .input-group input, .input-group select, .input-group textarea {
    width: 100%;
    padding: 10px;
    border: 1px solid #ddd;
    border-radius: 4px;
  }
  .submit-btn {
    width: 100%;
    padding: 10px;
    border: none;
    background-color: #5cb85c;
    color: white;
    font-size: 16px;
    cursor: pointer;
    border-radius: 4px;
  }
  .submit-btn:hover {
    background-color: #4cae4c;
  }
</style>
</head>
<body>

<div class="form-container">
  <h2>College Admission Form</h2>
  <form id="admissionForm">
    <div class="input-group">
      <label for="name">Full Name</label>
      <input type="text" id="name" name="name" required>
    </div>
    <div class="input-group">
      <label for="email">Email Address</label>
      <input type="email" id="email" name="email" required>
    </div>
    <div class="input-group">
      <label for="dob">Date of Birth</label>
      <input type="date" id="dob" name="dob" required>
    </div>
    <div class="input-group">
      <label for="gender">Gender</label>
      <select id="gender" name="gender" required>
        <option value="">Select Gender</option>
        <option value="male">Male</option>
        <option value="female">Female</option>
        <option value="other">Other</option>
      </select>
    </div>
    <div class="input-group">
      <label for="phone">Phone Number</label>
      <input type="tel" id="phone" name="phone" required>
    </div>
    <div class="input-group">
      <label for="address">Address</label>
      <textarea id="address" name="address" required></textarea>
    </div>
    <div class="input-group">
      <label for="city">City</label>
      <input type="text" id="city" name="city" required>
    </div>
    <div class="input-group">
      <label for="state">State/Province</label>
      <input type="text" id="state" name="state" required>
    </div>
    <div class="input-group">
      <label for="zip">ZIP/Postal Code</label>
      <input type="text" id="zip" name="zip" required>
    </div>
    <div class="input-group">
      <label for="country">Country</label>
      <select id="country" name="country" required>
        <option value="">Select Country</option>
        <!-- Add other countries as needed -->
      </select>
    </div>
    <div class="input-group">
      <label for="program">Program of Interest</label>
      <select id="program" name="program" required>
        <option value="">Select Program</option>
        <!-- Add programs as needed -->
      </select>
    </div>
    <div class="input-group">
      <label for="highschool">High School Name</label>
      <input type="text" id="highschool" name="highschool" required>
    </div>
    <div class="input-group">
      <label for="graduation">Expected Graduation Date</label>
      <input type="month" id="graduation" name="graduation" required>
    </div>
    <button type="submit" class="submit-btn">Submit Application</button>
  </form>
</div>

<script>
  document.getElementById('admissionForm').onsubmit = function(event) {
    event.preventDefault();
    // Here you would typically handle the form submission,
    // like sending the data to a server or validating input.
    alert('Application submitted successfully!');
  };
</script>

</body>
</html>
