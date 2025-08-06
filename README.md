<!DOCTYPE html>
<html>
<head>
  <title>Terima Kasih!</title>
</head>
<body>
  <h1>Terima kasih atas ketertarikanmu!</h1>
  <p>Halo <span id="namaUser"></span>, kami telah menerima data kamu.</p>
  <p>Tim kami akan menghubungi kamu segera via email.</p>

  <script>
    const urlParams = new URLSearchParams(window.location.search);
    const nama = urlParams.get('nama');
    document.getElementById('namaUser').textContent = nama || "kamu";
  </script>
</body>
</html>
