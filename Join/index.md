---
title: Join Us
nav:
  order: 6
  tooltip: Join the Team
---

# {% include icon.html icon="fa-solid fa-handshake-angle" %} Join the Team


<style>
  .contact-container {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    font-family: 'Arial', sans-serif;
    padding: 40px;
    background-color: #fff;
    max-width: 1000px;
    margin: auto;
    border-radius: 10px;
  }

  .left-column {
    width: 45%;
    padding-right: 40px;
  }

  .left-column h1 {
    font-size: 36px;
    margin-bottom: 10px;
    color: #333;
  }

  .left-column h2 {
    font-size: 18px;
    font-weight: bold;
    color: #444;
    margin-bottom: 15px;
  }

  .left-column p {
    font-size: 16px;
    line-height: 1.6;
    color: #333;
    margin: 5px 0;
  }

  .left-column em {
    font-style: italic;
    display: block;
    margin-top: 20px;
  }

  .left-column a {
    color: #000;
    text-decoration: none;
    font-weight: bold;
  }

  .right-column {
    width: 50%;
  }

  .form-group {
    margin-bottom: 20px;
  }

  label {
    display: block;
    font-size: 16px;
    margin-bottom: 5px;
    color: #c01f25;
  }

  input, textarea {
    width: 100%;
    padding: 12px;
    border: 1px solid #ccc;
    font-size: 16px;
    border-radius: 4px;
    background-color: #f8f8f8;
  }

  .name-fields {
    display: flex;
    gap: 10px;
  }

  .name-fields input {
    flex: 1;
  }

  button {
    padding: 12px 30px;
    background-color: #a8a39e;
    border: none;
    border-radius: 6px;
    color: white;
    font-size: 18px;
    cursor: pointer;
    margin-top: 10px;
  }

  .vertical-text {
    writing-mode: vertical-rl;
    transform: rotate(180deg);
    font-size: 32px;
    font-weight: bold;
    color: #c01f25;
    margin-right: 30px;
  }

  .contact-section {
    display: flex;
    align-items: flex-start;
  }
</style>

<div class="contact-section">
  <div class="vertical-text">Contact us</div>
  <div class="contact-container">

    <div class="left-column">
      <h1>Kelly Bolton Lab</h1>
      <h2>Washington University School of Medicine</h2>
      <p>Division of Oncology<br>
        Campus Box 8007<br>
        Washington University<br>
        660 South Euclid Avenue<br>
        St. Louis, MO 63110</p>

      <p>Room 5407C, 4444 Forest Park Blvd. (office)</p>

      <em>If you are interested in applying for a position in our lab, please contact:</em>
      <p><a href="mailto:bolton@wustl.edu">bolton@wustl.edu</a></p>
    </div>

    <div class="right-column">
      <form>
        <div class="form-group">
          <label for="name">Name <span style="color:gray;">(required)</span></label>
          <div class="name-fields">
            <input type="text" placeholder="First Name" required>
            <input type="text" placeholder="Last Name" required>
          </div>
        </div>
        <div class="form-group">
          <label for="email">Email <span style="color:gray;">(required)</span></label>
          <input type="email" placeholder="Your Email" required>
        </div>
        <div class="form-group">
          <label for="message">Message <span style="color:gray;">(required)</span></label>
          <textarea rows="5" placeholder="Your message..." required></textarea>
        </div>
        <button type="submit">Send</button>
      </form>
    </div>

  </div>
</div>
