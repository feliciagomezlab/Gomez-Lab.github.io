---
title: Join Us
nav:
  order: 6
  tooltip: Join the Team
---

# {% include icon.html icon="fa-solid fa-handshake-angle" %} Join the Team

<div class="join-us-container">
  <div class="contact-info">
    <h2>Felicia Gomez Lab</h2>
    <p>Washington University School of Medicine</p>
    <p>Division of Oncology</p>
    <p>Campus Box 8007</p>
    <p>Washington University</p>
    <p>660 South Euclid Avenue</p>
    <p>St. Louis, MO 63110</p>
    <p>Room 5407C, 4444 Forest Park Blvd. (office)</p>
    <p>If you are interested in applying for a position in our lab, please contact:</p>
    <p><a href="mailto:fgomez@wustl.edu">fgomez@wustl.edu</a></p>
  </div>
  <div class="contact-form">
    <h3>Contact Us</h3>
    <form action="https://formspree.io/f/feliciagomezlab" method="POST">
      <div class="form-group">
        <label for="name">Name (required)</label>
        <div class="name-fields">
          <input type="text" id="first-name" name="first-name" placeholder="First Name" required>
          <input type="text" id="last-name" name="last-name" placeholder="Last Name" required>
        </div>
      </div>
      <div class="form-group">
        <label for="email">Email (required)</label>
        <input type="email" id="email" name="email" placeholder="Email" required>
      </div>
      <div class="form-group">
        <label for="message">Message (required)</label>
        <textarea id="message" name="message" placeholder="Message" required></textarea>
      </div>
      <button type="submit">Send</button>
    </form>
  </div>
</div>

<style>
  .join-us-container {
    display: flex;
    justify-content: space-between;
    max-width: 900px;
    margin: 0 auto;
    padding: 30px;
  }
  .contact-info, .contact-form {
    flex: 1;
    padding: 20px;
  }
  .contact-info h2 {
    color: #333;
    margin-bottom: 15px;
    font-size: 1.5em;
  }
  .contact-info p {
    margin: 8px 0;
    color: #666;
    line-height: 1.5;
  }
  .contact-info a {
    color: #007bff;
    text-decoration: none;
  }
  .contact-form h3 {
    color: #800000;
    margin-bottom: 20px;
    font-size: 1.2em;
  }
  .form-group {
    margin-bottom: 20px;
  }
  .form-group label {
    display: block;
    color: #800000;
    margin-bottom: 5px;
    font-weight: bold;
  }
  .name-fields {
    display: flex;
    gap: 10px;
  }
  .name-fields input {
    flex: 1;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
    font-size: 1em;
  }
  .form-group input[type="email"], .form-group textarea {
    width: 100%;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
    font-size: 1em;
  }
  .form-group textarea {
    height: 120px;
    resize: vertical;
  }
  button {
    background-color: #999;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    font-size: 1em;
    margin-top: 10px;
  }
  button:hover {
    background-color: #777;
  }
  @media (max-width: 600px) {
    .join-us-container {
      flex-direction: column;
    }
    .contact-info, .contact-form {
      width: 100%;
    }
    .name-fields {
      flex-direction: column;
      gap: 10px;
    }
    .name-fields input {
      width: 100%;
    }
  }
</style>
