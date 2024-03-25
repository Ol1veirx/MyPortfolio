<template>
  <footer>
    <div class="footer-content">
      <div class="footer-box1">
          <a href="https://www.instagram.com/asppe.penedo/" target="_blank"><img src="" alt=""/></a>
          <span
            >Site desenvolvido por
            <a href="https://github.com/Ol1veirx" target="_blank"
              >Liedson Danúbio</a>
            </span>
      </div>
      <div class="footer-box2">
        <span>
            Email:<a href="mailto:liedsonleite3@hotmail.com">liedsonleite3@hotmail.com</a>
        </span>
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
  background-color: rgba(172, 255, 47, 0.281);
}


.footer-content p {
  color: black;
}

footer img {
  width: 30px;
}

@media (max-width: 768px) {
  .footer-content {
    font-size: 13px;
  }
}
</style>