   
  <html>
    <head>
      <style>
         
body {
	font-family: Arial, Helvetica, sans-serif;
  background-color: #EFB106;
	margin: 0;
	padding: 0;
}
.wrapper {
	width: 80%;
	margin: 0 auto;
	padding: 1em; 
	display: flex;
	flex-flow: row nowrap;
}
section {
	flex-basis: 57%;
	margin-right: 10%;
}
aside {
	flex-basis: 33%;
}
p, [for="abtype"] {
	margin-bottom: 0;
	margin-top: 2rem;
}
fieldset, #abtype {
	margin-bottom: 2rem;
} 
fieldset {
	border: 1px solid black;
	border-radius: 10px;
}
legend {
	font-weight: bold;
	font-size: 1.3rem;
	margin-top: 1.5rem;
	margin-bottom: 1rem;
	display: block;
}
label {
	display: block;
}
input:not([type="radio"]):not([type="checkbox"]), 
textarea {
	display: block;
	margin-bottom: 2rem;
	width: 20rem;
	font-family: Arial, Helvetica, sans-serif;
	font-size: 1em;
	border-radius: 10px;
	padding: 0 1rem;
}
textarea {
	height: 10rem;
	padding: 1rem;
}
select {
	font-size: 1rem;
}
button {
	margin: 2rem 0;
	background-color: #BB342F;
	color: white;
	border: none;
	font-size: 1rem;
	padding: 0.5rem 1rem;
	border-radius: 10px;
}
button:hover {
	background-color: #9A2B27;
}
        </style>
      </head>
    <body>  
	<div class="wrapper">
		<section>
      <h1>Kiran Fitness Gym</h1>
      <p>Fill out the form below to place an Registration</p>
			<form method="POST" action="https://e3vwdl4bpd.execute-api.us-west-2.amazonaws.com/default/API2SES">
				<fieldset>
					<legend>Your contact information</legend>
					<label for="name">Your name </label>
					<input type="text" id="name" name="name" autofocus>
					<label for="phone">Phone number</label>
					<input type="tel" id="phone" name="phone"  >
					<label for="email">Email</label>
					<input type="email" id="email" name="email">					 
          <label for="date">Joining date</label>
					<input type="date" id="date" name="date">
          <label for="qty">How many Months will you choose ?<label>
					<input type="number" id="qty" name="qty" min="1" max="12">
            <p>What type of training do you prefer?</p>
					<label>
						<input type="radio" name="ufotype" value="kk" checked>Body Intensity Training
					</label>
					<label>
						<input type="radio" name="ufotype" value="kk1"> Aerobic Interval Training
					</label>
					<label>
						<input type="radio" name="ufotype" value="kk2">Anaerobic Interval Training    
					</label>
					<label>
						<input type="radio" name="ufotype" value="kk3">Fartlek Training
					</label>
					<label>
						<input type="radio" name="ufotype" value="any">Circuit Training               
					</label>
					<label for="kiran">Type of Plans  </label>
					<select id="kiran" name="kiran">
            <option selected>Select one...</option>
						<option value="tour">1 Month $50             </option>
						<option value="dinner">3 Months $100 (save $50)   </option>
            <option value="dance">6 Months $225 (save $75)</option>
            <option value="whales">12 Months $500 (save $100)</option>
					</select>
			<label for="comments">Special requests:</label>
					<textarea id="comments" name="comments"></textarea>		 
			<input id="send_to" type="hidden" name="send_to" value="yourEmailHere">
					<button type="submit">Submit</button>
				</fieldset>
			</form>
		</section>
        <aside>
          <h1>Our Location</h1>
          <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3770.1091937159376!2d72.89627031421314!3d19.10286505609325!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3be7c9d98d504637%3A0x103babc83c2630b0!2sKiran%20Gym!5e0!3m2!1sen!2sin!4v1602441582199!5m2!1sen!2sin" width="300" height="250" frameborder="0" style="border:0;" allowfullscreen="" aria-hidden="false" tabindex="0"></iframe>"
		 <p>Subhash Nagar, Mohili, Asalpha, Mumbai, Maharashtra 400072</p>
	</div>
	<script src="js/forms.js"></script>   
</body>
</html>
