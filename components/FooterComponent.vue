<template>
  <div class="container">
    <div class="footer">
      <div class="left">
        <h2>Be the first to know</h2>
        <p>Sign up for updates from mettā muse.</p>
        <input type="text" placeholder="enter your email" />
        <button>Subscribe</button>
      </div>
      <div class="right">
        <h2>Be the first to know</h2>
        <ul>
          <li>+44 221 133 5360</li>
          <li>customercare@mettamuse.com</li>
        </ul>
        <div class="currency">
          <h2>Currency</h2>
          <img
            src="./../static/assets/United States of America (US).png"
            alt=""
          />
          <span>USD</span>
        </div>
        <p>
          Transactions will be completed in Euros and a currency reference is
          available on hover.
        </p>
      </div>
    </div>
    <div class="footer-two">
      <div class="left">
        <h2>mettā muse</h2>
        <ul>
          <li>About Us</li>
          <li>Stories</li>
          <li>Artisans</li>
          <li>Contact Us</li>
          <li>EU Compliances Docs</li>
        </ul>
      </div>
      <div class="middle">
        <h2>Quick Links</h2>
        <ul>
          <li>Orders & Shipping</li>
          <li>Join/Login as a Seller</li>
          <li>Payment & Pricing</li>
          <li>Return & Refunds</li>
          <li>FAQs</li>
          <li>Privacy Policy</li>
          <li>Terms & Conditions</li>
        </ul>
      </div>
      <div class="right">
        <h2>Follow Us</h2>
        <div class="social-media-icon">
          <img src="../static/assets/Insta.png" alt="" />
          <img src="../static/assets/a.png" alt="" />
        </div>
        <div class="payment-methods">
          <h2>mettā muse Accepts</h2>
          <img src="../static/assets/gpay.png" alt="" />
          <img src="../static/assets/mastercard.png" alt="" />
          <img src="../static/assets/paypal.png" alt="" />
          <img src="../static/assets/amex.png" alt="" />
          <img src="../static/assets/opay.png" alt="" />
        </div>
      </div>
    </div>
    <div class="copy-right">
      <p>Copyright © 2023 mettamuse. All rights reserved</p>
    </div>
  </div>
</template>
<script>
export default {}
</script>
<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.container {
  width: 100%;
  padding: 0%;
  margin: 0;
  /* max-width: 1440px; */
  background-color: #000;
  color: #fff;
}
.footer,
.footer-two {
  display: flex;
  flex-wrap: wrap;
  align-items: flex-start;
  justify-content: space-around;
  padding: 3% 3%;
  border-bottom: 1px solid #ffffff;
}
.footer-two {
  border-bottom: none;
}
.left h2,
.middle h2,
.right h2 {
  color: #fff;
}
.left button {
  background-color: #000;
  color: #ffffff;
  border: 2px solid #ffffff;
  padding: 5px;
}
.left input {
  padding: 5px;
}
.right ul li,
.middle ul li,
.left ul li {
  list-style: none;
  text-align: left;
}
.currency {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  gap: 2%;
}
.right p {
  font-family: 'Norm' sans-serif;
  font-size: 12px;
  font-weight: 400;
  line-height: 14.4px;
  text-align: left;
}
ul li {
  list-style: none;
  padding: 2%;
  line-height: 1.9em;
}
.copy-right {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 1% 1%;
}

@media (max-width: 768px) {
  .footer,
  .footer-two {
    flex-direction: column;
    align-items: center;
  }
  .footer .left,
  .footer .right,
  .footer-two .left,
  .footer-two .middle,
  .footer-two .right {
    width: 100%;
    text-align: center;
    margin-bottom: 20px;
  }
  .left input {
    width: 100%;
    margin-bottom: 10px;
  }
  .left button {
    width: 100%;
  }
}

@media (max-width: 480px) {
  .footer .left,
  .footer .right,
  .footer-two .left,
  .footer-two .middle,
  .footer-two .right {
    padding: 10px;
  }
  .right p,
  .currency h2,
  .currency span {
    font-size: 10px;
  }
  .currency img {
    width: 20px;
    height: 20px;
  }
  .social-media-icon img,
  .payment-methods img {
    width: 30px;
    height: 30px;
  }
}
</style>
