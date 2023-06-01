<template>
	<div class="body_wrap">
		<div class="dashboard_body mh-100">
			<div class="title_header d-flex mb_50 justify-content-between align-items-center">
				<h1 class="text-left title ">All Offers</h1> 
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
					<thead>
						<tr>
							<th scope="col " class="w40">
								<div class="checkbox_wrap">
									<input type="checkbox" name="iagree_to_be_contacted" id="news-regarding" class="">
									<label for="news-regarding" class="f14 text-white"> </label>
								</div>
							</th>
							<th scope="col" class="f16 lit_clr">Offer Code</th>
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
							<th scope="col" class="f16 lit_clr"><a href="" class="lit_clr">Last Updated <img src="../../../assets/images/arrow_down.png" alt="arrow_down" class="ml-2"></a></th>
							<th scope="col" class="f16 lit_clr">Status</th>
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
							<td class="f14">SHUKRI25</td>
							<td class="f14">Al Rifai Roastery</td>
							<td class="f14">2022-06-23 19:30:04</td>
							<td class="f14"><span class="bage">No Expiry</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>
						<tr>
							<th>
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="two" class="">
									<label for="two" class="f14 text-white"> </label>
								</div>
							</th>
							<td class="f14">CAKE4ME</td>
							<td class="f14">Cake Boutique Cafe</td>
							<td class="f14">2022-06-23 23:49:03</td>
							<td class="f14"><span class="bage">No Expiry</span></td>
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
							<td class="f14">SHUKRI456</td>
							<td class="f14">Carrefour</td>
							<td class="f14">2022-06-23 23:51:29</td>
							<td class="f14"><span class="bage-success">Active</span></td>
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
							<td class="f14">PIZZAPIZZA</td>
							<td class="f14">Papa Johns</td>
							<td class="f14">2022-06-23 19:30:04</td>
							<td class="f14"><span class="bage-success">Active</span></td>
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
							<td class="f14">SHUKRIBUCKET</td>
							<td class="f14">Samui Thai Restaurant</td>
							<td class="f14">2022-06-23 23:49:03</td>
							<td class="f14"><span class="bage-success">Active</span></td>
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
							<td class="f14">MSHUKRI</td>
							<td class="f14">McDonald’s</td>
							<td class="f14">2022-06-23 23:51:29</td>
							<td class="f14"><span class="bage-danger">Expired</span></td>
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
							<td class="f14">SHUKRI20</td>
							<td class="f14">Carrefour</td>
							<td class="f14">2022-06-23 19:30:04</td>
							<td class="f14"><span class="bage-danger">Expired</span></td>
							<td class="f14">
								<div class="action_btn"> <a href="#" class="f16 txt_b"><span><Edit/></span>Edit</a> </div>
							</td>
						</tr>
						<tr>
							<th>
								<div class="checkbox_wrap">
									<input type="checkbox" name="table" id="8th" class="">
									<label for="8th" class="f14 text-white"> </label>
								</div>
							</th>
							<td class="f14">SHURKI123</td>
							<td class="f14">SHURKI123</td>
							<td class="f14">2022-06-23 19:30:04</td>
							<td class="f14"><span class="bage-info">Draft</span></td>
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
												<p class="mb-0"><b>Showing 1 to 10 of 56 results</b></p>
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
   name:'AllOffer',
   components: {
    Search,Edit
  },
  }
 </script>
 
 
 
 
 
 
 <style >
  
 </style>
 