# abc
<!Doctype HTML>
<html>
<head><title>registration form</title>
 <link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.6.3/css/font-awesome.min.css" rel="stylesheet" integrity="sha384-T8Gy5hrqNKT+hzMclPo118YTQO6cYprQmhrYwIiQ/3axmI1hQomh7Ud2hPOy8SP1" crossorigin="anonymous">
    <link rel="stylesheet"href="https://maxcdn.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
    
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js"></script>
          <meta charset="utf-8">
          <meta name="viewport" content="width=device-width,initial-scale=1">
	<style>
		body{
			background-image:linear-gradient(to right,rgb(217,122,28),rgb(227,197,30));
	
			height:1500px;
			
			width:100%;
		
		}   
	
	
		.container{
			background-color:white;
		     margin-top:90px;
			padding-right:60px;
			padding-left:50px;
		    width:50%;
			height:1100px;
			border:3px solid black; 
			box-shadow:20px 20px  20px rgb(255,85,0);
			
			
		}
	
		#q{
	     color:black;
		  box-shadow: 7px 7px 5px grey;
		  font-weight:bold;
		}
		#p{
	     color:black;
		  box-shadow: 7px 7px 5px grey;
		  font-weight:bold;
		}#r{
	     color:black;
		  box-shadow: 7px 7px 5px grey;
		  font-weight:bold;
		}#s{
	     color:black;
		  box-shadow: 7px 7px 5px grey;
		  font-weight:bold;
		}#t{
	     color:black;
		  box-shadow: 7px 7px 5px grey;
		  font-weight:bold;
		}#u{
	     color:black;
		  box-shadow: 7px 7px 5px grey;
		  font-weight:bold;
		}
		textarea{
			border:2px solid black;
		}
	
		button{
			margin-left:230px;
			margin-top: 40px;
		}
	
	
	
	</style></head>
	<body>
	
	
	<div class="container">
		
		<h1 style="color:brown;padding-top:25px"><b><i>...REGISTRATION FORM...</i></b></h1>
		<p style="float:right"><i>!!here u starts your journey  with us....</i></p>
		
		<br>
		
	
		<form onsubmit="return validation()" id="rupform">
			<div class="form-group">
				<label for="name"><b>NAME:</b></label>
				<input type="text" name="name" class="form-control" id="p">
			</div>
			<div class="form-group">
            <label for="email" ><b>EMAIL:</b></label>
				<input type="text" name="email" class="form-control" id="q"	>
			</div>
			
				<div class="form-group">
            <label for="address" ><b>ADDRESS:</b></label>
				<input type="text" class="form-control" id="r" name="address">
			</div>
			<div class="form-group">
            <label for="phoneno" ><b>PHONE NUMBER:</b></label>
				<input type="text"class="form-control"  id="s" name="phone number" maxlenght="10"	>
			</div>
			     
			<div class="form-group">
            <label for="dob" ><b>DATE OF BIRTH:</b></label>
				<input type="text" class="form-control"  id="t"name="dob">
			</div>
			<div class="form-group form-radio">
            <label for="password" ><b>PASSWORD:</b></label>
				<input type="password" class="form-control"  name="password"id="u">
			</div>
			
				<div class="form-group">
				
		     <label for="gender"><b>GENDER:</b></label>
					<ul>
				<input type="radio"  name="gender" value="female"id="female">FEMALE<br>
				<input type="radio"  name="gender" value="male" id="male">MALE<br>
			<input type="radio"  name="gender" value="others"id="others">OTHERS<br>
		 
					</ul>
	
				</div>
			
			
			<div class="form-group form-check">
				<label class="form-check-label" ><b>INTERESTS:</b></label>
				<ul>
				<input type="checkbox" class="form-check-input" name="option" value="designing" id="l">DESIGNING<br>
			<input type="checkbox" class="form-check-input" name="option" value="hacking"id="l" >HACKING<br>
			<input type="checkbox" class="form-check-input" name="option" value="content writing" id="l">CONTENT WRITING<br>
					<input type="checkbox" class="form-check-input" name="option" value="authoring" id="l">PUBLIC AUTHORING<br></ul></div>
			
			<div class="form-group">
			<label for="textarea"><b>SUGGESTIONS:</b></label>
				
				
			<textarea rows="5" cols="50" style="float:right;text-align: left" id="io">
				
				
				
				</textarea>			
			
			
			</div>
		
			<input type="submit" value="submit">
			
			</form>
		
          
		</div>
		<script>
		var x=document.forms["rupform"];
			function validation(){
				if(x["p"].value==""){
					alert("please provide your name");
					x["p"].focus();
					return false;
				}
				
				if(x["q"].value==""){
					alert("provide your email");
					x["q"].focus();
				return false;
				}
				
                 if(x["r"].value==""){
					alert("provide your address");
					x["r"].focus();
				return false;
				}
				 if(x["s"].value==""){
					alert("provide your phone no");
					x["s"].focus();
				return false;
				}
                  if(x["t"].value==""){
					alert("provide  your dob");
					x["t"].focus();
				return false;
				}
				 if(x["u"].value==""){
					alert("provide your password");
					x["u"].focus();
				return false;
				}
				var genders=document.getElementsByName["gender"];
				if(genders[0].checked==true){
					alert(" you are female");
					
				}
				else if(genders[1].checked==true){
					alert("you are male ");
					
				}
				else if(genders[2].checked==true){
					 alert("you are from others ");
					
				}else{
					  alert("plz choose one of these");
                    return false;
				}

		
				
				
				var t;
				var checkbox=document.querySelectorAll('input[type="checkbox"]');
				var checkboxch=Array.prototype.slice.call(checkbox).some(t=>t.checked);
				if(!checkboxch){
					alert("please provide  your choice");
					return false;
				}
				if(x["io"].value==""){
					alert("plz fill suggestion box");
					x["io"].focus();
				return false;
				}
				
				
				
				
				var first=x["p"].value;
				var regName= /^[A-Za-z]+$/ ;
				if(!first.match(regName)){
					alert("invalid  name");
					x["p"].focus();
						return false;
						
					
				}
				var emailID=x["q"].value;
				var atpos=emailID.indexof("@");
				var dotpos=emailIDindexof(".");
				if(atpos < 1 || ( dopos - atpos < 2)){
					alert("please enter the right email");
					x["q"].focus();
					return false;
					
				}
				var phone=x["s"].value;
				var phoneNum= /^\(?([0-9]{3})\)?([0-9]{3})[-. ]?([0-9]{4})$/;
				if(!phone.match(phoneNum)){
					alert("invalid phone number");
					x["s"].focus();
					return false;
				}
				var dob=x["t"].value;
				var dateReg = /^\d{2}[./-]\d{2}[./-]\d{4}$/;
				if(!dob.match(dateReg)){
					alert("invalid dob");
					x["t"].focus();
					return false;
					
				}
				var passwords=x["u"].value;
				var pattern=/^(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).*$/;
				if(!passwords.match(pattern)){
					alert("invalid  password");
					x["u"].focus();
					return false;
					
				}
			 
	
		</script>	
			
		   
	
	
	
	
	
	
	
	</body>
</html>
