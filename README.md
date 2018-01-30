# validation-form-using-JS
<!DOCTYPE html>
<head>  
<title>JavaScript Validation Form</title> 
</head>

<body>
<h2>Log In Member</h2>
<input type="text" name="username" id="username" placeholder="Username...">
<input type="password" name="password" id="password" placeholder="Password...">

<button id="button_login" onclick="validation();">Log In</button>
<p id="notice"></p>

<script type="text/javascript">
  var validation = function(){
  var username = document.getElementById('username').value;
  var password = document.getElementById('password').value;
  
  var old_username = "webdeveloper";
  var old_password = "hello!gb";
  
  if(username == '' && password == ''){
    document.getElementById('notice').innerHTML = 'Your fields still blank out';
  }
  
  else {  
    if(username == old_username && password == old_password){
      document.getElementById('notice').innerHTML = 'You successful login!';
    }
    else{
     document.getElementById('notice').innerHTML = 'Your password and username wrong!';   
    }
  }
  
  console.log(username);
  }
  </script>
  </body>
  </html>
  
  
