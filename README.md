<!DOCTYPE html>
<html>
    <head>
     <title>
         intern_web Screens - Figma
     </title>
     <link rel="stylesheet" href="style.css">

     
      <script type="text/javascript">
        function Validate() 
        {
          var password = document.getElementById("txtPassword").value;
          var confirmPassword = document.getElementById("txtConfirmPassword").value;
        if (password != confirmPassword) 
        {
           alert("Passwords do not match.");
           return false;
        }
          return true;
        }
      </script>


   </head>
    <body style="background-image: url('intern.jpg');" id="checkinput">
        
        <div class="container">
            <div class="h">Imaginnovate </div>
            <div id= "title"> Register your account</div>
        
          <form name="myform" class="content">
             <div class="input-box" id="name1">
                 <span class="details" id="firstname">First Name</span>
                 <input type="text"  placeholder="Enter your First name" onblur="validation();" required>
             </div>
             <div class="input-box" id="name2">
                 <span class="details" id="lastname">Last Name</span>
                 <input type="text" placeholder="Enter your Last name" onblur="validation();" required >
               </div>

              <div class="input-box" id="number">
                 <span class="details" id="phonenumber">Phone Number</span>
                 <input type="number"  placeholder="Enter your Phone Number"  minlength="10" maxlength="10" onblur="validation();" required>
              </div>
              <div class="input-box" id="mail">
                 <span class="details" id="email" >Email</span>
                <input type="email" placeholder="Enter your Email" onblur="validation();" required>
              </div>

              
              <form>
                <lablel class="input-box" id="password" id="form" action="">
                  <span class="details" id="message" >Password</span>
                  <input type="password"  onblur="return validation" placeholder="Enter your Password" pattern="(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{8,}" title="Must contain at least one number and one uppercase and lowercase letter, and at least 8 or more characters"  onblur="validation();"required >
                </lablel>
              
                <label class="input-box" id="confirm_password">
                 <span class="details" id="message" >Confirm Password</span>
                 <input type="password" onblur="return validation" placeholder="Enter your Confirm Password" pattern="(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{8,}" title="Must contain at least one number and one uppercase and lowercase letter, and at least 8 or more characters"  onblur="validation();"required >
                </form>
              
              <input type="radio" name="terms" value="terms & conditions" >I agree to Terms & Privacy Policy
              <div class="submit">
                <input type="submit" value="Create Account" >
              </div>  
              
              <div id="text">
                <p>Dont have an account? Join free today</p>          
              </div>

              

           </form>
 
        </div> 
    </body>
    
</html>
  
