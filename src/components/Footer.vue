<template>
  <footer>
    <div class="footer-content">
      <div class="footer-box1">
          <a href="https://www.instagram.com/asppe.penedo/" target="_blank"><img src="" alt=""/></a>
          <span>Copyright © 2024 by Liedson Danúbio. All rights reserved.</span>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "MyFooter",
};
</script>

<style scoped>
footer {
  padding: 15px;
  background-color: #c97309;
}


.footer-content p {
  color: black;
}

.footer-box1 span {
  font-weight: bold;
}

footer img {
  width: 30px;
}

@media (max-width: 768px) {
  footer{
    display: none;
  }
  .footer-content {
    font-size: 13px;
  }
}
</style>