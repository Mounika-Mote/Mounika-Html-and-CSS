# Mounika-Html-and-CSS
<!DOCTYPE html>
<html>
<head>
    <title>Registration Form</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js"></script>
    <link rel="stylesheet" href="login.css">
    <style>
        .text1
        {
            color:red;
        }
        .text2
        {
            color:green;
        }
    </style>
    <script>
        $(document).ready(function(){
            $("#reg").submit(function(e){
                e.preventDefault();
                var email=$("#email").val();
                var password=$("#pass").val();
                if(email=="")
                {
                    $("#msg5").html("Enter Your email");
                }
                else if(password=="")
                {
                    $("#msg5").html("Enter Your password");
                }
                else
                {
                    $("#msg5").html("Success");
                    m.reset();

                }
            });
        });
    </script>
</head>
<body>
<div class="container ">
    <div class="jumbotron div1">
        <form action="" id="reg" class="form-vertical">
            <div class="form-group">
                <label>Email:</label>
                <input type="email" class="form-control" id="email">
                <p id="msg2"></p>
            </div>
            <div class="form-group">
                <label>Password:</label>
                <input type="password" class="form-control" id="pass">
                <p id="msg3"></p>
                <input type="submit" value="submit()" class="btn btn-success">
                <p id="msg4"></p>
            </div>
            <p id="msg5"></p>
        </form>
        <hr>
        <center>
            <a href="registration.html" class="btn btn-success">Create New Account</a>
        </center>
    </div>
</div>
</body>
