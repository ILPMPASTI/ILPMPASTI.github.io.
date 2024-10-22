# ILPMPASTI.github.io.
<!DOCTYPE html>
<html>
<head>
    <title>Pengesahan AuthPro</title>
    <script type="text/javascript" src="https://www.authpro.com/auth/accesstool.js"></script>
    <script>
        // Fungsi untuk memeriksa akses pengguna
        function checkAuth() {
            if (authpro_accesstool.checkAccess()) {
                document.getElementById("auth-message").innerHTML = "Akses dibenarkan.";
            } else {
                document.getElementById("auth-message").innerHTML = "Anda tidak mempunyai akses.";
            }
        }
    </script>
</head>
<body onload="checkAuth()">
    <h1>Halaman Dilindungi</h1>
    <div id="auth-message"></div>
</body>
</html>
