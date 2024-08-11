

```html
<script>
  if (confirm("Are you randi?")) {
    document.body.innerHTML += "<h1 style='color: green; font-size: 40px; animation: blink 1s infinite;'>Gud bhosdiwali</h1>";
  } else {
    document.body.innerHTML += "<h1 style='color: red; font-size: 40px;'>Randi hai bhosdiwali</h1>";
  }
</script>
<style>
  @keyframes blink {
    50% { opacity: 0; }
  }
</style>
   
