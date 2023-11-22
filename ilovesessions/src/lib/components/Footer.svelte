<script>

</script>

<footer class="footer">
    <div class="footer-container">
      <div class="footer-logo">
        <a href="#"><img src="image.jpg" alt="Logo"></a>
      </div>
  
      <div class="footer-navigation">
        <ul>
          <li><a href="#">About Us</a></li>
          <li><a href="#">Contact Us</a></li>
          <li><a href="#">Privacy Policy</a></li>
          <li><a href="#">Terms of Service</a></li>
        </ul>
      </div>
  
      <div class="footer-copyright">
        <p>&copy; 2023 Your Company Name. All rights reserved.</p>
      </div>
    </div>
  </footer>

<style>
.footer {
  background-color: #f2f2f2;
  padding: 30px;
  text-align: center;
}

.footer-container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.footer-logo {
  margin-bottom: 20px;
}

.footer-navigation ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

.footer-navigation li {
  display: inline-block;
  margin-right: 10px;
}

.footer-navigation a {
  text-decoration: none;
  color: #333;
}

.footer-copyright {
  margin-top: 20px;
  font-size: 12px;
  color: #999;
}

@media (max-width: 768px) {
  .footer-container {
    flex-direction: column-reverse;
  }

  .footer-navigation ul {
    text-align: left;
  }
}
</style>