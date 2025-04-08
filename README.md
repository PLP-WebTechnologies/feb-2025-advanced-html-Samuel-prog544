# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Index Page</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f2f2f2;
      margin: 20px;
      padding: 20px;
    }

    h2 {
      color: #333;
    }

    img {
      max-width: 100%;
      height: auto;
      margin-bottom: 20px;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      margin-bottom: 30px;
    }

    table, th, td {
      border: 1px solid #999;
    }

    th, td {
      padding: 10px;
      text-align: left;
    }

    form {
      background-color: #fff;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      max-width: 600px;
    }

    label {
      display: block;
      margin-top: 15px;
      font-weight: bold;
    }

    input, select {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }

    .form-section {
      margin-top: 20px;
    }

    .form-group-inline {
      display: flex;
      gap: 10px;
    }

    .form-group-inline label {
      font-weight: normal;
      margin-left: 5px;
    }

    button {
      margin-top: 20px;
      padding: 10px 20px;
      background-color: #4CAF50;
      color: #fff;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    button:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>

  <!-- Title -->
  <h2>Ordered List (Roman Numerals)</h2>
  <!-- Ordered list with Roman numerals -->
  <ol type="I">
    <li>Home</li>
    <li>About</li>
    <li>Projects</li>
    <li>Gallery</li>
    <li>Contact</li>
  </ol>

  <!-- External image from Pexels -->
  <h2>Sample Image</h2>
  <img src="https://images.pexels.com/photos/3183150/pexels-photo-3183150.jpeg" alt="Office Setup from Pexels" />

  <!-- Contact Table -->
  <h2>Contact List</h2>
  <table>
    <thead>
      <tr>
        <th>Name</th>
        <th>Address</th>
        <th>Mobile</th>
        <th>Email</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Jane Doe</td>
        <td>Nairobi, Kenya</td>
        <td>+254 712345678</td>
        <td>jane@example.com</td>
      </tr>
      <tr>
        <td>John Smith</td>
        <td>Mombasa, Kenya</td>
        <td>+254 798765432</td>
        <td>john@example.com</td>
      </tr>
      <tr>
        <td>Alice Mwangi</td>
        <td>Kisumu, Kenya</td>
        <td>+254 701234567</td>
        <td>alice@example.com</td>
      </tr>
      <tr>
        <td>Brian Otieno</td>
        <td>Nakuru, Kenya</td>
        <td>+254 700987654</td>
        <td>brian@example.com</td>
      </tr>
      <tr>
        <td>Susan Karanja</td>
        <td>Eldoret, Kenya</td>
        <td>+254 723456789</td>
        <td>susan@example.com</td>
      </tr>
    </tbody>
  </table>

  <!-- Registration Form -->
  <h2>Registration Form</h2>
  <form action="#" method="post">
    <!-- Name -->
    <label for="name">Full Name *</label>
    <input type="text" id="name" name="name" placeholder="Enter your full name" required />

    <!-- Email -->
    <label for="email">Email Address *</label>
    <input type="email" id="email" name="email" placeholder="example@domain.com" required />

    <!-- Password -->
    <label for="password">Password *</label>
    <input type="password" id="password" name="password" placeholder="Create a password" minlength="6" required />

    <!-- Date of Birth -->
    <label for="dob">Date of Birth *</label>
    <input type="date" id="dob" name="dob" required />

    <!-- Dropdown (Country) -->
    <label for="country">Select Your Country *</label>
    <select id="country" name="country" required>
      <option value="">-- Select Country --</option>
      <option value="kenya">Kenya</option>
      <option value="uganda">Uganda</option>
      <option value="tanzania">Tanzania</option>
      <option value="rwanda">Rwanda</option>
    </select>

    <!-- Gender (Radio Buttons) -->
    <div class="form-section">
      <label>Gender *</label>
      <div class="form-group-inline">
        <input type="radio" id="male" name="gender" value="male" required />
        <label for="male">Male</label>
        <input type="radio" id="female" name="gender" value="female" />
        <label for="female">Female</label>
        <input type="radio" id="other" name="gender" value="other" />
        <label for="other">Other</label>
      </div>
    </div>

    <!-- Interests (Checkboxes) -->
    <div class="form-section">
      <label>Interests</label>
      <div class="form-group-inline">
        <input type="checkbox" id="coding" name="interests" value="coding" />
        <label for="coding">Coding</label>
        <input type="checkbox" id="design" name="interests" value="design" />
        <label for="design">Design</label>
        <input type="checkbox
