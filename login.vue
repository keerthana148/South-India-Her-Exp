<template>
    <div class="Login Form">
        
        <div class="login-page">
            <div class="form">
                <form class="resgister-form">
                <input type="text" placeholder="user name"/>
                <input type="text" placeholder="password"/>  
                <input type="text" placeholder="email id"/> 
                <a href="details.vue"> 
                <button>Create</button> 
                </a>
                <p class ="meassge">Already Registered? <a href ="#"> Login</a></p>   
                </form>
                <form class ="login form">
                <input type="text" placeholder="user name"/>
                <input type="password" placeholder="password"/>
                < a href="details.vue">
                <button> login</button>
                </a>
                <p class ="message">Not Registered?<a href ="#">Register</a></p>7
                </form>
            </div>   
        </div>
        <script src='https://code.jquery.com/jquery-3.4.1.min.js'></script>
        <script>
            $('.message a').click(function(){
                $('form').animate({height: "toggle",opacity:"toggle"},"slow");
            });
        </script>
    </div>    
</template> 
<style scoped>
body
{
    background-image: linear-gradient(rgba(0,0,0,0.6),rgba(0,0,0,0.6)),url(img.jpg);
    height: 100vh;
    background-size: cover;
    background-position: center;
}
.login-page 
{
    width: 360px;
    padding: 10% 0 0;
    margin: auto;
}
.form
{
    position: relative;
    z-index: 1;
    background: rgba(7, 40, 195, 0.8);
    max-width: 360px;
    margin: 0 auto 100px;
    padding: 45px;
    text-align: center;
}
.form input
{
   font-family: sans-serif;
   outline: 1;
   background: #f2f2f2;
   width: 100%;
   border: 0;
   margin: 0 0 15px;
   padding: 15px;
   box-sizing: border-box;
   font-size:  14px;

}
.form button
{
    font-family: sans-serif;
    text-transform: uppercase;
    outline: 0;
    background: #4caf50;
    width: 100%;
    border: 0;
    padding: 15px;
    color: #ffffff;
    font-size: 14px;
    cursor: pointer;
}
.form button:hover,.form button:active
{
    background: #43a047;
}
.form .message
{
    margin: 15px 0 0;
    color: aliceblue;
    font-size: 12px;
}
.form .message a
{
    color: #4caf50;
    text-decoration: none;
}
.form .register-form
{
    display: none;
}
<script>       
    
