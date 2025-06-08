<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Vendia - Your Style, Your Choice</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: #fafafa;
      margin: 0;
      padding: 20px;
      color: #222;
      display: flex;
      flex-direction: column;
      align-items: center;
      min-height: 100vh;
    }
    header {
      max-width: 600px;
      width: 100%;
      text-align: center;
      margin-bottom: 30px;
    }
    header h1 {
      font-weight: 700;
      color: #111;
      letter-spacing: 1.5px;
      margin-bottom: 6px;
    }
    header p {
      color: #555;
      font-size: 0.9rem;
    }
    .product-card {
      background: #fff;
      border-radius: 8px;
      box-shadow: 0 3px 12px rgb(0 0 0 / 0.1);
      width: 100%;
      max-width: 400px;
      padding: 24px;
      box-sizing: border-box;
      margin-bottom: 20px;
    }
    .product-card h2[contenteditable="true"] {
      border-bottom: 1px dashed #ccc;
      padding: 6px 0;
      cursor: text;
      font-size: 1.5rem;
      margin-bottom: 16px;
    }
    p, ul, h3 {
      margin: 8px 0;
    }
    [contenteditable="true"] {
      outline: none;
      padding: 2px 6px;
      border-radius: 3px;
      border: 1px solid transparent;
      transition: border-color 0.2s ease;
      cursor: text;
      display: inline-block;
      min-width: 20px;
    }
    [contenteditable="true"]:focus {
      border-color: #1a73e8;
      background-color: #e8f0fe;
    }
    hr {
      border: none;
      border-top: 1px solid #ddd;
      margin: 20px 0;
    }
    ul {
      padding-left: 20px;
      list-style: none;
    }
    ul li {
      margin-bottom: 8px;
    }
    a {
      color: #1a73e8;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
    button {
      cursor: pointer;
      background-color: #1a73e8;
      color: white;
      border: none;
      padding: 10px 20px;
      border-radius: 6px;
      font-size: 1rem;
      margin-top: 10px;
      transition: background-color 0.3s ease;
    }
    button:hover {
      background-color: #155ab6;
    }
    #cart {
      max-width: 400px;
      width: 100%;
      background: #fff;
      border-radius: 8px;
      box-shadow: 0 3px 12px rgb(0 0 0 / 0.1);
      padding: 20px;
      box-sizing: border-box;
      margin-top: 10px;
      display: none;
    }
    #cart h3 {
      margin-top: 0;
      margin-bottom: 10px;
    }
    #cart ul {
      padding-left: 20px;
      margin-bottom: 10px;
    }
    #cart ul li {
      margin-bottom: 6px;
    }
    footer {
      margin-top: auto;
      font-size: 0.85rem;
      color: #888;
      text-align: center;
      width: 100%;
      max-width: 600px;
      padding: 20px 0 10px;
    }
  </style>
</head>
<body>

  <header>
    <h1>Vendia</h1>
    <p>Your Style, Your Choice — Shop with ease</p>
  </header>

  <main>
    <div class="product-card">
      <h2 contenteditable="true" class="product-title">Product Title</h2>

      <p><strong>Size:</strong> <span contenteditable="true" id="product-size">L</span></p>
      <p><strong>Price:</strong> ₹<span contenteditable="true" id="product-price">750</span></p>

      <hr />

      <h3>🛍️ How to Buy:</h3>
      <ul>
        <li>✅ <strong>Add to Cart</strong> – Secure online checkout</li>
        <li>✅ <strong>Cash on Delivery</strong> – On orders above ₹350</li>
        <li>
          ✅ <strong>DM to Buy:</strong><br />
          • <a href="https://www.instagram.com/_vendia._" target="_blank">Message on Instagram</a><br />
          • <a id="whatsapp-link" href="#" target="_blank">Chat on WhatsApp</a>
        </li>
      </ul>

      <hr />

      <p>📦 <strong>Pan India Delivery:</strong> 9–10 working days</p>
      <p>🚚 <strong>Free Shipping:</strong> On all retail orders</p>
      <p>💳 <strong>Payment Modes:</strong> UPI, Net Banking, Credit/Debit Card, Google Pay, PhonePe, Paytm</p>

      <p>📲 <strong>Follow us:</strong> <a href="https://www.instagram.com/_vendia._" target="_blank">@_.vendia._</a></p>

      <button id="add-to-cart-btn">Add to Cart</button>
    </div>

    <div id="cart">
      <h3>Your Cart</h3>
      <ul id="cart-items"></ul>
      <p><strong>Total:</strong> ₹<span id="cart-total">0</span></p>
      <button id="checkout-btn">Proceed to Checkout</button>
      <button id="clear-cart-btn" style="background:#e53935; margin-left:10px;">Clear Cart</button>
    </div>
  </main>

  <footer# Vendia
