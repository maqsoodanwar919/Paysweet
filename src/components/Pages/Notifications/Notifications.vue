<template>
	<div class="body_wrap">
		<div class="dashboard_body mh-100">
			<div class="title_header d-flex mb_50 justify-content-between align-items-center">
				<h1 class="text-left title ">Notifications</h1>
				<button type="button" class="btn theme-btn2 w185 "><span>New Notification</span></button>
			</div>
			<div class="custom_table user_table">
				<div class="row table_search_filter align-items-center justify-content-between">
					<div class="col-3">
						<div class="form-group mb_25">
							<label class="mb_6 f14">Status</label>
							<select class="form-control custom_select">
								<option>All</option>
							</select>
						</div>
					</div>
					<div class="col-2 text-end ml-auto "> <a href="#" class="linke_reest a_over">Reset filters</a> </div>
				</div>
				<table class="table mb-0">
					<thead class="bg_head border_head">
						<tr>
							<th scope="col" class="w40">
								<div class="checkbox_wrap">
									<input type="checkbox" name="iagree_to_be_contacted" id="news-regarding" class="">
									<label for="news-regarding" class="f14 text-white"> </label>
								</div>
							</th>
							<th scope="col" class="f16 lit_clr">ID</th>
							<th scope="col" class="f16 lit_clr"> Title </th>
							<th scope="col" class="f16 lit_clr">Message</th>
							<th scope="col" class="f16 lit_clr">Last Updated</th>
							<th scope="col" class="f16 lit_clr"> Status</th> 
						</tr>
					</thead>
					<tbody>
						<tr>
							<td class="f14">
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="one" class="">
									<label for="one" class="f14 text-white"> </label>
								</div>
							</td>
							<td class="f14">Free Pizza 🍕</td>
							<td class="f14">It ain’t easy being cheesy. Get 25% offer on...</td>
							<td class="f14">2022-06-23 19:30:04</td>
							<td class="f14"><span class="bage">Draft</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>
						<tr>
							<td class="f14">
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="two" class="">
									<label for="two" class="f14 text-white"> </label>
								</div>
							</td>
							<td class="f14">Best of Bahrain’s Burgers 🍔</td>
							<td class="f14">Join me and find the best burger spots in...</td>
							<td class="f14">2022-06-23 23:49:03</td>
							<td class="f14"><span class="bage">Draft</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>
						<tr>
							<td class="f14">
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="3th" class="">
									<label for="3th" class="f14 text-white"> </label>
								</div>
							</td>
							<td class="f14">يوم العالمي للتكة</td>
							<td class="f14">تعالو معاي نجيك فطيرة شكري</td>
							<td class="f14">2022-06-23 23:51:29</td>
							<td class="f14"><span class="bage-success">Published</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>
						<tr>
							<td class="f14">
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="4th" class="">
									<label for="4th" class="f14 text-white"> </label>
								</div>
							</td>
							<td class="f14">Shukri x Milkd 🍦</td>
							<td class="f14">Try my new flavour for the summer</td>
							<td class="f14">2022-06-23 19:30:04</td>
							<td class="f14"><span class="bage-success">Published</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>
						<tr>
							<td class="f14">
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="5th" class="">
									<label for="5th" class="f14 text-white"> </label>
								</div>
							</td>
							<td class="f14">Valentine’s Day Offer 😍</td>
							<td class="f14">The places to go for a date night 🌹</td>
							<td class="f14">2022-06-23 23:49:03</td>
							<td class="f14"><span class="bage-success">Published</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>
						<tr>
							<td class="f14">
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="6th" class="">
									<label for="6th" class="f14 text-white"> </label>
								</div>
							</td>
							<td class="f14">New Restaurants 💛</td>
							<td class="f14">Got new reviews, new menus, new items 👀</td>
							<td class="f14">2022-06-23 23:51:29</td>
							<td class="f14"><span class="bage-success">Published</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>
						<tr>
							<td class="f14">
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="7th" class="">
									<label for="7th" class="f14 text-white"> </label>
								</div>
							</td>
							<td class="f14">iknowhatoeat in Dubai 🇦🇪</td>
							<td class="f14">Going to new places</td>
							<td class="f14">2022-06-23 19:30:04</td>
							<td class="f14"><span class="bage">Draft</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>

						<tr>
							<td class="f14">
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="8th" class="">
									<label for="8th" class="f14 text-white"> </label>
								</div>
							</td>
							<td class="f14">Where to go this weekend?</td>
							<td class="f14">Find the best places for this hot weekend</td>
							<td class="f14">2022-06-23 19:30:04</td>
							<td class="f14"><span class="bage">Draft</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>



						<tr>
							<td class="f14">
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="9th" class="">
									<label for="9th" class="f14 text-white"> </label>
								</div>
							</td>
							<td class="f14">Got plans?</td>
							<td class="f14">Use ‘Surprise Me’ to find where to eat</td>
							<td class="f14">2022-06-23 23:51:29</td>
							<td class="f14"><span class="bage">Draft</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>


						<tr>
							<td class="f14">
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="10th" class="">
									<label for="10th" class="f14 text-white"> </label>
								</div>
							</td>
							<td class="f14">National Day Offers</td>
							<td class="f14">iknowhatoeat do you?</td>
							<td class="f14">2022-06-23 23:51:29</td>
							<td class="f14"><span class="bage-success">Published</span></td>
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
											<div class="table_footer d-flex justify-content-between align-items-center table_pd">
												<p class="mb-0"><b>Showing 1 to 10 of 108 results</b></p>
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
 
 



 <script>  
  import Search from '../../../assets/images/icon/search.vue';
 import Edit from '../../../assets/images/icon/edit.vue';
  export default{
   name:'Notifications',
   components: {
    Search,Edit
  },
  }
 </script>
 
 
 
 
 
 
 <style scoped>
  
 </style>
 