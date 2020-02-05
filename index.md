<!DOCTYPE html>
<html lang="en">
<head>
  <title>Kiosk Escape 1.1</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
  <style type="text/css">
  .jumbotron {
  	background-image: url('background.jpg');
  	background-repeat: no-repeat;
  	background-position: top;
  	background-size: 100% 600px;
  	height: 600px;
  }
  </style>
</head>
<body>

<div class="jumbotron text-center">
  <!-- h1>Kiosk Escape Tool</h1>
  <p>v1.1</p -->
</div>

<div class="container">
  <div class="row">
    <div class="col-sm-4">
    <h3>System Information</h3>
      <div id="diagnostic"></div>
        <p><script>
        var txt = "";
        txt += "<p>Browser CodeName: " + navigator.appCodeName + "</p>";
        txt += "<p>Browser Name: " + navigator.appName + "</p>";
        txt += "<p>Browser Version: " + navigator.appVersion + "</p>";
        txt += "<p>Cookies Enabled: " + navigator.cookieEnabled + "</p>";
        txt += "<p>Browser Language: " + navigator.language + "</p>";
        txt += "<p>Browser Online: " + navigator.onLine + "</p>";
        txt += "<p>Platform: " + navigator.platform + "</p>";
        txt += "<p>User-agent header: " + navigator.userAgent + "</p>";

        document.getElementById("diagnostic").innerHTML = txt;

        </script></p>
      </div>
    <div class="col-sm-4">
      <h3>Internal Links</h3>
      <a href="File:/C:/windows">File:/C:/windows</a>><br>
      <a href="File:/C:\windows\">File:/C:\windows\</a><br>
      <a href="File:/C:\windows/">File:/C:\windows/</a><br>
      <a href="File:/C:/windows">File:/C:/windows</a><br>
      <a href="File://C:/windows">File://C:/windows</a><br>
      <a href="File://C:\windows/">File://C:\windows/</a><br> 
      <a href="file://C:\windows">file://C:\windows</a><br> 
      <a href="C:/windows">C:/windows</a><br>
      <a href="C:\windows\">C:\windows\</a><br> 
      <a href="C:\windows">C:\windows</a><br> 
      <a href="C:/windows/">C:/windows/</a><br> 
      <a href="C:/windows\">C:/windows\</a><br>
      <a href="%WINDIR%">%WINDIR%</a><br> 
      <a href="%TMP%">%TMP%</a><br> 
      <a href="%TEMP%">%TEMP%</a><br> 
      <a href="%SYSTEMDRIVE%">%SYSTEMDRIVE%</a><br>
      <a href="%SYSTEMROOT%">%SYSTEMROOT%</a><br>
      <a href="%APPDATA%">%APPDATA%</a><br> 
      <a href="%HOMEDRIVE%">%HOMEDRIVE%</a><br>  
      <a href="%HOMESHARE%">%HOMESHARE%</a><br>
      <a href="Callto://">Callto</a><br>
      <a href="Gopher://">Gopher</a><br>
      <a href="HCP://">HCP</a><br>
      <a href="Telnet://">Telnet</a><br>
      <a href="TN3270://">TN3270</a><br> 
      <a href="Rlogin://">Rlogin</a><br>
      <a href="LDAP://">LDAP</a><br> 
      <a href="News://">News</a><br>
      <a href="Mailto://">Mailto</a><br>
    </div>
    <div class="col-sm-4">
      <h3>Shortcuts</h3>
      <p>CTRL-B, CTRL-I (Favourites)</p><br>
      <p>CTRL-H (History)</p><br>
      <p>CTRL-L, CTL-0 (File/Open Dialog)</p><br> 
      <p>CTRL-P (Print Dialog)</p><br>
      <p>CTRL-S (Save As)</p><br>
      <input type="file">
      <br>

      <button onclick="printSpawn()">Spawn print dialogue</button>
      <script>
      function printSpawn() {
          window.print();
      }
      </script>
    </div>
  </div>
  <div class="row">
    <div class="col-sm-12">
    <h3>Plugins</h3>
    <p><table border="1">
         <tr>
            <th>Plug-in Name</th>
            <th>Filename</th>
            <th>Description</th>
         </tr>
         
         <script language="JavaScript" type="text/javascript">
            for (i=0; i<navigator.plugins.length; i++) {
               document.write("<tr><td>");
               document.write(navigator.plugins[i].name);
               document.write("</td><td>");
               document.write(navigator.plugins[i].filename);
               document.write("</td><td>");
               document.write(navigator.plugins[i].description);
               document.write("</td></tr>");
            }
         </script>
         
      </table></p>
  </div>
</div>
</body>
</html>
