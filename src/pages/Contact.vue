<template>
  <Layout :show-logo="true">
    
		<div class="contact text-center">
			<h1>Contact Simon</h1>

			<section>
				<h4>Send Comments or Questions</h4>

				<div class="container">
					<form action="https://formspree.io/xzbjbkdy"
						method="POST"
					>
						<div class="form-row">
							<div class="col-25">
								<label for="fname">Your email</label>
							</div>
							<div class="col-75">
								<input id="fname" type="text" name="_replyto" placeholder="Email">
							</div>
						</div>
						
						<div class="form-row">
							<div class="col-25">
								<label for="subject">Message</label>
							</div>
							<div class="col-75">
								<textarea id="subject" name="message" placeholder="Questions or Comments" style="height:200px"></textarea>
							</div>
						</div>
						<div class="form-row text-center">
							<input type="submit" value="Submit" />
						</div>
					</form>
				</div>

			</section>
		</div>
  </Layout>
</template>

<style lang="scss" scoped>
	.contact {
		height: 90vh;
		padding: 2em;
	}
	
	* {
  box-sizing: border-box;
}

input[type=text], textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 4px;
	resize: vertical;	
	margin-bottom: 2em;
}

label {
  padding: 12px 12px 12px 0;
	display: inline-block;
	color: black;
}

input[type=submit] {
  background-color: var(--link-color);
	color: black;
	font-weight: 800;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
	cursor: pointer;
	float: right;
}

input[type=submit]:hover {
	background-color: var(--link-color);
	color: white;
}

.container {
  border-radius: 5px;
  background-color: #b84040;
  padding: 20px;
}

.col-25 {
  float: left;
  width: 25%;
  margin-top: 6px;
}

.col-75 {
  float: left;
  width: 75%;
  margin-top: 6px;
}

/* Clear floats after the columns */
.form-row:after {
  content: "";
  display: table;
  clear: both;
}

/* Responsive layout - when the screen is less than 600px wide, make the two columns stack on top of each other instead of next to each other */
@media screen and (max-width: 640px) {
  .col-25, .col-75, input[type=submit] {
    width: 100%;
    margin-top: 0;
  }
}
</style>