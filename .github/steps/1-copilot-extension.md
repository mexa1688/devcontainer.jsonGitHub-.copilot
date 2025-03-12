<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Daily Skincare Routine Survey Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f4f4f9;
      margin: 0;
      padding: 20px;
    }
    #title {
      color: #2c3e50;
      text-align: center;
    }
    #description {
      text-align: center;
      font-size: 1.2em;
      color: #7f8c8d;
    }
    form {
      max-width: 600px;
      margin: 0 auto;
      padding: 20px;
      background-color: white;
      border-radius: 8px;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    }
    label {
      display: block;
      margin: 10px 0 5px;
      font-weight: bold;
    }
    input, select, textarea {
      width: 100%;
      padding: 10px;
      margin-bottom: 20px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }
    input[type="number"] {
      -moz-appearance: textfield;
    }
    input[type="number"]::-webkit-outer-spin-button, 
    input[type="number"]::-webkit-inner-spin-button {
      -webkit-appearance: none;
      margin: 0;
    }
    button {
      background-color: #3498db;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      font-size: 1.1em;
    }
    button:hover {
      background-color: #2980b9;
    }
  </style>
</head>
<body>

  <h1 id="title">Daily Skincare Routine Survey Form</h1>

  <p id="description">In this survey, you will share about your daily skincare routine.</p>

  <form id="survey-form">
    <!-- Name Input -->
    <label id="name-label" for="name">Name:</label>
    <input type="text" id="name" name="name" placeholder="Enter your name" required>

    <!-- Email Input -->
    <label id="email-label" for="email">Email:</label>
    <input type="email" id="email" name="email" placeholder="Enter your email" required>

    <!-- Number Input -->
    <label id="number-label" for="number">Age:</label>
    <input type="number" id="number" name="age" placeholder="Enter your age" min="18" max="100" required>

    <!-- Dropdown Select -->
    <label for="dropdown">Favorite Skincare Product:</label>
    <select id="dropdown" name="product" required>
      <option value="">Select a product</option>
      <option value="moisturizer">Moisturizer</option>
      <option value="sunscreen">Sunscreen</option>
      <option value="cleanser">Cleanser</option>
      <option value="serum">Serum</option>
    </select>

    <!-- Radio Buttons -->
    <label>Skin Type:</label>
    <input type="radio" id="oily" name="skin-type" value="oily">
    <label for="oily">Oily</label>
    <input type="radio" id="dry" name="skin-type" value="dry">
    <label for="dry">Dry</label>
    <input type="radio" id="combination" name="skin-type" value="combination">
    <label for="combination">Combination</label>

    <!-- Checkboxes -->
    <label>Which steps do you follow in your skincare routine?</label>
    <input type="checkbox" id="cleanse" name="steps" value="cleanse">
    <label for="cleanse">Cleansing</label>
    <input type="checkbox" id="tone" name="steps" value="tone">
    <label for="tone">Toning</label>
    <input type="checkbox" id="moisturize" name="steps" value="moisturize">
    <label for="moisturize">Moisturizing</label>
    <input type="checkbox" id="sunscreen" name="steps" value="sunscreen">
    <label for="sunscreen">Sunscreen</label>

    <!-- Textarea -->
    <label for="comments">Additional Comments:</label>
    <textarea id="comments" name="comments" rows="4" placeholder="Leave your comments here..."></textarea>

    <!-- Submit Button -->
    <button id="submit" type="submit">Submit</button>
  </form>

</body>
</html>
