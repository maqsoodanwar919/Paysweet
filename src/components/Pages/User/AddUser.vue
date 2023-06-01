

<template> 
<div class="body_wrap">
	<div class="dashboard_body mh-100">
		<h1 class="text-left title mb_50">Create New User</h1>
		<form class="" action="">
			<div class="row">
				<div class="col-md-5">
					<div class="form-group mb_25">
						<label class="mb_6 f14">Name</label>
						<input type="text" class="form-control" placeholder="Enter name" /> </div>
				</div>
				<div class="col-md-5">
					<div class="form-group mb_25">
						<label class="mb_6 f14">Email</label>
						<input type="email" class="form-control" placeholder="Enter email address" /> </div>
				</div>
				<div class="col-md-5">
					<div class="form-group mb_25">
						<label class="mb_6 f14">User Type</label>
						<select class="form-control custom_select">
							<option>Select an option</option>
						</select>
					</div>
				</div>
				<div class="col-md-5">
					<div class="form-group mb_25">
						<label class="mb_6 f14">Password</label>
						<input type="email" class="form-control" placeholder="Enter password" /> </div>
				</div>
			</div>
			<div class="theme_btn_wrap mt_30">
				<button type="button" class="btn theme-btn2 mr_10"><span>Save</span></button>
				<button type="button" class="btn theme-btn-white"><span>Cancel</span></button>
			</div>
		</form>
	</div>
</div>
   
   
 </template>
 
 
 



 <script>  
  export default{
   name:'AddUser',
    
  }
 </script>
 
 
 
 
 
 
 <style scoped>
  
 </style>
 