<template>
	<div class="body_wrap">
		<div class="dashboard_body mh-100">
			<div class="title_header d-flex mb_50 justify-content-between align-items-center">
				<h1 class="text-left title ">Users & Admin</h1>
				<button type="button" class="btn theme-btn2   "><span>New User</span></button>
			</div>
			<div class="custom_table user_table">
				<table class="table mb-0">
					<thead>
						<tr>
							<th scope="col " class="w40">
								<div class="checkbox_wrap">
									<input type="checkbox" name="iagree_to_be_contacted" id="news-regarding" class="">
									<label for="news-regarding" class="f14 text-white"> </label>
								</div>
							</th>
							<th scope="col" class="f16 lit_clr">ID</th>
							<th scope="col">
								<form class="form_tabel">
									<div class="form-group mb-0">
										<div class="icon_wrap">
											<input type="email" class="form-control pl_40" placeholder="Enter name…" />
											<div class="icon">
												<Search /> </div>
										</div>
									</div>
								</form>
							</th>
							<th scope="col" class="f16 lit_clr">Email</th>
							<th scope="col" class="f16 lit_clr">User Type</th>
							<th scope="col" class="f16 lit_clr"> </th>
						</tr>
					</thead>
					<tbody>
						<tr>
							<th>
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="one" class="">
									<label for="one" class="f14 text-white"> </label>
								</div>
							</th>
							<td class="f14">1</td>
							<td class="f14">Maryam Shukri</td>
							<td class="f14">maryam.shukri@example.com</td>
							<td class="f14"><span class="bage">Admin</span></td>
							<td class="f14"></td>
						</tr>
						<tr>
							<th>
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="two" class="">
									<label for="two" class="f14 text-white"> </label>
								</div>
							</th>
							<td class="f14">2</td>
							<td class="f14">Ahmed Mohamed</td>
							<td class="f14">ahmed1005@example.com</td>
							<td class="f14"><span class="bage">Editor</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>
						<tr>
							<th>
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="3th" class="">
									<label for="3th" class="f14 text-white"> </label>
								</div>
							</th>
							<td class="f14">3</td>
							<td class="f14">Hasan Maki</td>
							<td class="f14">hasan.maki@example.com</td>
							<td class="f14"><span class="bage">Editor</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>
						<tr>
							<th>
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="4th" class="">
									<label for="4th" class="f14 text-white"> </label>
								</div>
							</th>
							<td class="f14">4</td>
							<td class="f14">Hasan Maki</td>
							<td class="f14">hasan.maki@example.com</td>
							<td class="f14"><span class="bage">Editor</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>
						<tr>
							<th>
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="10th" class="">
									<label for="10th" class="f14 text-white"> </label>
								</div>
							</th>
							<td class="f14">5</td>
							<td class="f14">Ryan Ekstrom</td>
							<td class="f14">ryan.e.s.123@example.com</td>
							<td class="f14"><span class="bage">Editor</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>
						<tr>
							<th>
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="9th" class="">
									<label for="9th" class="f14 text-white"> </label>
								</div>
							</th>
							<td class="f14">6</td>
							<td class="f14">Gustavo Herwitz</td>
							<td class="f14">gustavo.hertz@example.com</td>
							<td class="f14"><span class="bage">Editor</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>
						<tr>
							<th>
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="7th" class="">
									<label for="7th" class="f14 text-white"> </label>
								</div>
							</th>
							<td class="f14">7</td>
							<td class="f14">Cooper Culhane</td>
							<td class="f14">cooper9057313@example.com</td>
							<td class="f14"><span class="bage">Editor</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>
					</tbody>
					<tfoot>
						<tr>
							<td colspan="6">
								<table class="w-100">
									<tr>
										<td>
											<div class="table_footer d-flex justify-content-between align-items-center">
												<p class="mb-0"><b>Showing 1 to 7 of 7 results</b></p>
												<div class="pages_wrap d-flex  align-items-center mr-2">
													<div class="select">
														<select name="format" id="format">
															<option value="">1</option>
															<option value="">2</option>
															<option value="">3</option>
															<option value="">4</option>
															<option value="">5</option>
															<option value="">6</option>
															<option value="">7</option>
															<option value="">8</option>
															<option value="">9</option>
															<option value="">10</option>
														</select>
													</div> <span class="f14 ">per page</span> </div>
												<div class="table_pagination">
													<!-- ewew -->
												</div>
											</div>
										</td>
									</tr>
								</table>
							</td>
						</tr>
					</tfoot>
				</table>
			</div>
		</div>
	</div>
</template>
 
 
 



 <script >  
 import Search from '../../../assets/images/icon/search.vue';
 import Edit from '../../../assets/images/icon/edit.vue';
   export default{
   name:'user',
   components: {
    Search,Edit
  },
  }
 </script>
 
 
 
 
 
 
 <style >
  
 </style>
 