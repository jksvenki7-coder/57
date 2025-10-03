# 57<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>JKS Group of Business</title>
<style>
  body {font-family: Arial, sans-serif; background-color: #f0f8ff; margin: 0; padding: 0; color:#333;}
  header {background: #87ceeb; padding: 20px; text-align: center; color: white;}
  h1 {margin: 0;}
  section {padding: 20px; margin: 10px;}
  h2 {color: #005f87; border-bottom: 2px solid #87ceeb; padding-bottom: 5px;}
  .service-group {background: white; border-radius: 8px; padding: 15px; margin-bottom: 20px; box-shadow: 0 0 6px #ccc;}
  form {margin-top: 10px;}
  label {display: block; margin: 8px 0 4px;}
  input, textarea, select {width: 100%; padding: 8px; box-sizing: border-box; border: 1px solid #ccc; border-radius: 4px;}
  button {background-color: #005f87; color: white; border: none; padding: 10px 15px; cursor: pointer; border-radius: 4px;}
  button:hover {background-color: #004a65;}
  .map-container {width: 100%; height: 300px; background: #ddd; border-radius: 8px; margin-top: 10px; display: flex; justify-content: center; align-items: center; color: #555;}
  a.whatsapp-link {color: #25D366; font-weight: bold; text-decoration: none;}
</style>
</head>
<body>

<header>
  <h1>JKS Group of Business</h1>
  <p>Multi-service Platform - All-in-One</p>
</header>

<section>
  <h2>Advertisement & Survey</h2>
  <div class="service-group">
    <ul>
      <li>Influencer Marketing</li>
      <li>Social Media Marketing</li>
      <li>Banner Ads (Pamphlet Distribution, Posters on Walls)</li>
      <li>Cycling Ads</li>
      <li>Drone Ads</li>
      <li>Vehicle Ads</li>
      <li>Video Making & Editing</li>
      <li>Poster Design</li>
      <li>Voice Over</li>
    </ul>
    <h3>Request a Service</h3>
    <form id="advertisementForm">
      <label for="adServiceName">Service</label>
      <input type="text" id="adServiceName" name="adServiceName" placeholder="Enter advertisement service" required />
      <label for="adDetails">Details</label>
      <textarea id="adDetails" name="adDetails" placeholder="Enter service details or questions" required></textarea>
      <button type="submit">Submit Advertisement Request</button>
    </form>
  </div>
</section>

<section>
  <h2>Events & Catering</h2>
  <div class="service-group">
    <h3>Packages (Price details shown)</h3>
    <ul>
      <li>Birthday Party Package - ₹5000</li>
      <li>Wedding Package - ₹50000</li>
      <li>Corporate Event Package - ₹20000</li>
    </ul>
    <h3>Customized Services (Budget & Capacity input)</h3>
    <form id="customizedServicesForm">
      <label for="serviceName">Service Name</label>
      <input type="text" id="serviceName" name="serviceName" placeholder="Enter service" required />
      <label for="budget">Budget (₹)</label>
      <input type="number" id="budget" name="budget" placeholder="Enter your budget" required />
      <label for="capacity">Capacity (Number of people)</label>
      <input type="number" id="capacity" name="capacity" placeholder="Enter capacity" required />
      <button type="submit">Submit Customized Service Request</button>
    </form>
    <h3>Premium Services (Open details form only - no budget or capacity)</h3>
    <form id="premiumServiceForm">
      <label for="premiumService">Service</label>
      <input type="text" id="premiumService" name="premiumService" placeholder="Enter premium service" required />
      <label for="details">Details</label>
      <textarea id="details" name="details" placeholder="Enter your details" required></textarea>
      <button type="submit">Submit Premium Service Request</button>
    </form>
  </div>
</section>

<section>
  <h2>E-commerce (Groceries, Food, Pharmacy)</h2>
  <div class="service-group">
    <ul>
      <li>Groceries Folder: Rice, Pulses, Spices</li>
      <li>Food Folder: Snacks, Sweets, Frozen Foods</li>
      <li>Pharmacy Folder: Medicines, Health Supplements</li>
    </ul>
  </div>
</section>

<section>
  <h2>Other Services</h2>
  <div class="service-group">
    <ul>
      <li>Job Consultancy</li>
      <li>Courier Booking</li>
      <li>Loans & Insurance Services</li>
      <li>Tours & Travels</li>
      <li>Real Estate Services</li>
      <li>Home & Handyman Services</li>
      <li>Investment Advisory Services</li>
    </ul>
  </div>
</section>

<section>
  <h2>Recharge & Bill Payment</h2>
  <form id="rechargeForm">
    <label for="mobileNumber">Mobile Number</label>
    <input type="tel" id="mobileNumber" name="mobileNumber" placeholder="Enter mobile number" required />
    <label for="amount">Amount (₹)</label>
    <input type="number" id="amount" name="amount" placeholder="Enter amount" required />
    <button type="submit">Pay Now</button>
  </form>
</section>

<section>
  <h2>Contact & Ordering</h2>
  <p>Contact us or place your orders through WhatsApp:</p>
  <p><a class="whatsapp-link" href="https://wa.me/918977143043" target="_blank">Chat on WhatsApp: 8977143043</a></p>
  
  <h3>Order Details Form</h3>
  <form id="orderForm">
    <label for="customerName">Name</label>
    <input type="text" id="customerName" name="customerName" placeholder="Enter your name" required />
    <label for="customerMobile">Mobile Number</label>
    <input type="tel" id="customerMobile" name="customerMobile" placeholder="Enter your mobile number" required />
    <label for="orderDetails">Order Details</label>
    <textarea id="orderDetails" name="orderDetails" placeholder="Enter order details" required></textarea>
    <label for="deliveryAddress">Delivery Address</label>
    <textarea id="deliveryAddress" name="deliveryAddress" placeholder="Enter delivery address" required></textarea>
    <button type="submit">Submit Order</button>
  </form>
</section>

<section>
  <h2>Location Finder</h2>
  <div class="map-container" id="googleMapPlaceholder">
    Google Maps will be integrated here.
  </div>
</section>

<script>
  document.getElementById('advertisementForm').addEventListener('submit', function(e) {
    e.preventDefault();
    alert('Advertisement Service Request Submitted');
  });
  document.getElementById('customizedServicesForm').addEventListener('submit', function(e) {
    e.preventDefault();
    alert('Customized Service Request Submitted');
  });
  document.getElementById('premiumServiceForm').addEventListener('submit', function(e) {
    e.preventDefault();
    alert('Premium Service Request Submitted');
  });
  document.getElementById('rechargeForm').addEventListener('submit', function(e) {
    e.preventDefault();
    alert('Recharge Payment Submitted');
  });
  document.getElementById('orderForm').addEventListener('submit', function(e) {
    e.preventDefault();
    alert('Order Submitted');
  });
</script>

</body>
</html>
