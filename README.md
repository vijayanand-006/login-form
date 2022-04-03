<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Login form</title>
</head>
<style type="text/css">
  *
  {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  body
  {
    background: #121212;
    height: 100vh;
    font-family: sans-serif,serif,cursive;
    display: grid;
    place-items:center;
  }
  form
  {
    text-align: center;
    background: #ffff;
    width: auto;
    display: flex;
    flex-direction: column;
    margin: auto;
    padding: 2rem 4rem;
    border-radius: 20px;
  }
  input[type="email"],input[type="password"]
  {
    margin: 10px;
    padding: 10px;
    border-radius: 5px;
  }
  input[type="email"]:focus
  {
    outline-color:black;
  }
  input[type="submit"]
  {
    width: 100%;
    margin: 10px;
    padding: 5px;
    border: none;
    position: relative;
    border-radius: 30px;
    color: white;
    background-color: blue;
  }
  #p
  {
    margin: 10px;
    position: relative;
    right: 30px;
  }
  #p1
  {
      margin: 10px;
      position: relative;
      right: 30px;
  }
</style>
<body>
<form action="#" id="login"> 
  <h1>Ocean Blue</h1>
  <input type="email" id="email" placeholder="Email" required/>  <!--type email required-->
  <input type="password" name="pass" placeholder="password" required/> <!--type password required-->
  <p id="p"><a href="#">forgot password?</a></p> <!--forgot password-->
  <input type="submit" value="Login"/> <!-- submit button -->
  <p id="#p1">Create an account?<a href="#">Signup</a></p> 
</form>

<script>
  const form = document.querySelector("#login");

  form.addEventListener("button", function (e) {
    e.preventDefault();
    console.log("Form submitted!");
  });

</script>
</body>
</html>
