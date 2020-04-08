---
title: Academic Projects

# The About page
# v2.0
# https://github.com/cotes2020/jekyll-theme-chirpy
# © 2017-2019 Cotes Chung
# MIT License
---
<head>
	<style>
		.container-portfolio { 
			position: relative; 
			width: 100%; 
			margin: 0 auto; 
			-webkit-transition: all 1s ease;
			-moz-transition: all 1s ease;
			-o-transition: all 1s ease;
			transition: all 1s ease;	
		}

		#filters {
			margin:1%;
			padding:0;
			list-style:none;
			display: inline-block;

		}

		#filters li {
			float:left;
			text-align: center;
		}

		#filters li span {
			display: block;
			padding:5px 20px;		
			text-decoration:none;
			color:#fff;
			cursor: pointer;
			background: #577285;
			margin: 2px;
		}

		#filters li span.active {
			color:#fff;
		}

		#portfoliolist .portfolio {
			-webkit-box-sizing: border-box;
			-moz-box-sizing: border-box;
			-o-box-sizing: border-box;
			width:31%;
			margin:1%;
			display:none;
			float:left;
			overflow:hidden;
		}

		.portfolio-wrapper {
			overflow:hidden;
			position: relative !important;
			background: #666;
			cursor:pointer;
		}

		.portfolio img {
			max-width:100%;
			position: relative;
		}

		.portfolio .label {
			position: absolute;
			width: 100%;
			height:40px;
			bottom:-40px;
			display: block !important;
		}

		.portfolio .label-bg {
			width: 100%;
			height:100%;
			position: absolute;
			top:0;
			left:0;
		}

		.portfolio .label-text {
			color:#fff;
			position: relative;
			z-index:500;
			padding:5px 8px;
			font-weight:300;
		}

		.portfolio .text-title {
			display:block;
			font-size:13px;
			margin: 1px;
			color : #fff;
			text-transform:capitalize;
		}
		#fancybox-title {
			margin-left: 10px !important;
			width: 380px !important;
			bottom: 10px !important;
			display: block !important;
		}


		@media only screen and (max-width: 767px) {

			#portfoliolist .portfolio {
				width:48%;
				margin:1%;
			}	

			.widget-profil,
			.flexy_content {
				margin-left: 10px;
				margin-right: 10px;
			}

		}

		@media only screen and (max-width: 550px) {

			#filters li  {
				width: 100%;
			}

			#profile .cycle-slideshow {
				display: none;
			}

		}

		/* #Clearing */
		/* Self Clearing Goodness */
		.container:after { content: "\0020"; display: block; height: 0; clear: both; visibility: hidden; }

		.clearfix:before,
		.clearfix:after,
		.row:before,
		.row:after {
			content: '\0020';
			display: block;
			overflow: hidden;
			visibility: hidden;
			width: 0;
			height: 0; }
		.row:after,
		.clearfix:after {
			clear: both; }
		.row,
		.clearfix {
			zoom: 1; }

		.clear {
			clear: both;
			display: block;
			overflow: hidden;
			visibility: hidden;
			width: 0;
			height: 0;
		}
		#profile .about i.glyphicon  {
			margin-right: 3px;
		}

		#profile .profile-r {
			padding-right: 0;
		}
		#profile .cycle-slideshow {
			margin-top: 19px;
			margin-bottom: 20px;
			width: 348px;
			height: 456px;
		}
		#profile .cycle-slideshow img {
			width: 100%;
		}
		.bottom-p .panel-body {
			padding: 15px;
			color: #999 !important;
			font-size: 14px;
			font-family: 'Lato', sans-serif;
		}
		.bottom-p .panel-group .panel {
			border-radius:0px;
		}

		.bottom-p .panel-heading {
			border-top-right-radius: 0px;
			border-top-left-radius: 0px;
		}

		ul.about li span.value {
			width: 220px;
			text-align: left;
			float: right;
		}
		ul.about li {
			margin: 0;
			color: #717171;
			display: block;
			font-size: 13px;
			border-bottom: 1px solid #e6e6e6;
		}

		ul.about li:last-child {
			border-bottom: none;
		}
		ul.about {
			margin-bottom: 30px;
		}

		#profile .bottom-p  {
			margin-top: 20px;
		}

		#profile .bottom-p p {
			border-left:0;
		}


		#profile .bottom-p h3 {
			margin-top: 60px;
			margin-bottom: 20px;
		}
		/** style profile 3 **/
		.ch-grid-prof {
			margin: 20px 0 0 0;
			padding: 0;
			list-style: none;
			display: block;
			text-align: center;
			width: 100%;
		}
		.ch-grid-prof:after, .ch-item-prof:before {
			content: '';
			display: table;
		}
		.ch-grid-prof:after {
			clear: both;
		}
		.ch-grid-prof li {
			width: 220px;
			height: 220px;
			display: inline-block;
			margin: 20px;
		}
		.ch-items-prof {
			width: 150px;
			height: 150px;
			border-radius: 50%;
			overflow: hidden;
			position: relative;
			cursor: default;
			box-shadow: inset 0 0 0 5px rgba(255,255,255,0.6), 0 1px 2px rgba(0,0,0,0.1);
			box-shadow: inset 0 0 0 3px rgba(255,255,255,0.6), 0 1px 2px rgba(0,0,0,0.1);
			transition: all 0.4s ease-in-out;
			margin: 0 auto;
			margin-bottom: 10px;
		}
		.ch-info-prof {
			position: absolute;
			width: inherit;
			height: inherit;
			border-radius: 50%;
			overflow: hidden;
			opacity: 0;
			transition: all 0.4s ease-in-out;
			transform: scale(0);
		}
		.ch-info-prof h3 {
			color: #fff;
			text-transform: uppercase;
			letter-spacing: 2px;
			font-size: 25px;
			margin: 0 auto;
			padding: 50px 0 0 0;
			text-shadow: 0 0 1px #fff, 0 1px 2px rgba(0,0,0,0.3);
			line-height: 22px;
			border: none;
		}
		.ch-info-prof p {
			color: #fff;
			padding: 10px 5px;
			font-style: italic;
			margin: 0 30px;
			font-size: 12px;
			border-top: 1px solid rgba(255,255,255,0.5);
			opacity: 0;
			transition: all 1s ease-in-out 0.4s;
		}
		.ch-info-prof p a {
			display: block;
			color: rgba(255,255,255,0.7);
			font-style: normal;
			text-transform: uppercase;
			font-size: 9px;
			letter-spacing: 1px;
			padding-top: 4px;
		}
		.ch-info-prof p a:hover {
			color: rgba(255,242,34, 0.8);
		}
		.ch-items-prof:hover {
			box-shadow: inset 0 0 0 1px rgba(255,255,255,0.1), 0 1px 2px rgba(0,0,0,0.1);
		}
		.ch-items-prof:hover .ch-info-prof {
			transform: scale(1);
			opacity: 1;
		}
		.ch-items-prof:hover .ch-info-prof p {
			opacity: 1;
		}
		.content_2 {
			height: 580px;
			-webkit-box-sizing:border-box;
			-moz-box-sizing:border-box;
			box-sizing:border-box;		
		}
		.bottom-p .panel-body {
			padding: 11px;
			font-size: 11px;
			text-align: justify;
		}
		.panel-title {
			font-size: 13px;
		}
		.panel{
			border:none !important;	
		}
	</style>
</head>

<div id="portfolio" class="content_2">
<!-- service 2 -->
	<div class="row">
		<div class="col-md-12">
			<div class="bottom-p">
				<div class="panel-group" id="accordion">
					<div class="panel panel-default">
						<div class="panel-heading">
							<h4 class="panel-title">
								<a data-toggle="collapse" data-parent="#accordion" href="#collapseOne" class="collapse_tabs">
									Data Analysis in R - Kickstarter Projects Success Prediction
									<i class="glyphicon glyphicon-chevron-up" style="float: right;font-size: 13px;"></i>
								</a>
							</h4>
						</div>
						<div id="collapseOne" class="panel-collapse collapse in">
							<div class="panel-body">
								<i class="fa fa-quote-left"></i> Skills acquired: Data analysis, data visualization, team management <br>
								Tools: R, Weka, PowerBI, MS Word, MS Powerpoint <br>

								Collaborated in a team of 3 people, I gathered project requirements to ensure success for Kickstarter project launchers. Consistently met deadlines with project team, allocated tasks and followed the agile Kanban methodology using the Trello app. Moreover, we generated visualizations for the data using PowerBI to show region wise and category wise factors for project success. Finally, we predicted factors which contribute to Kaggle project success based on models such as Decision trees, Random forests, Naïve Bayes classification, Clustering analysis, Support vector machine, Logistic regression and Association rule mining to validate analysis and find answers to data questions.                    </div>
							</div>
						</div>
					
					<div class="panel panel-default">
						<div class="panel-heading">
							<h4 class="panel-title">
								<a data-toggle="collapse" data-parent="#accordion" href="#collapseTwo" class="collapse_tabs">
									Database Management in SQL - Health Care Portal
									<i class="glyphicon glyphicon-chevron-down" style="float: right;font-size: 13px;"></i>
								</a>
							</h4>
						</div>
						<div id="collapseTwo" class="panel-collapse collapse">
							<div class="panel-body">
								<i class="fa fa-quote-left"></i>  Skills acquired: Database management, data administration <br>
								Tools: MS SQL Server Management Studio, MS Access, MS Visio, MS Word <br> 
								Communicated with healthcare center to gather requirements and summarized knowledge about existing healthcare portal and identified shortcomings in the existing system, documented business suggestions and developed system design using MS Visio. We developed a new system using MS SQL Server management studio for database and MS Access for creating front end. Also, we increased the system accuracy and reducing human load by automating appointment process and bill generation processes.
							</div>
						</div>
					</div>
					
					<div class="panel panel-default">
						<div class="panel-heading">
							<h4 class="panel-title">
								<a data-toggle="collapse" data-parent="#accordion" href="#collapseThree" class="collapse_tabs">
								Data Analytics in Google Analytics - Whitman School of Management Website
								<i class="glyphicon glyphicon-chevron-down" style="float: right;font-size: 13px;"></i>
								</a>
							</h4>
						</div>
						<div id="collapseThree" class="panel-collapse collapse">
							<div class="panel-body">
								<i class="fa fa-quote-left"></i> Skills acquired: Web data analysis <br>
								Tools used: Google Analytics <br>
								Utilizing Google Analytics, I tracked the behavior, demographics and devices used by visitors to suggest correct target audience. Also, I evaluated areas for improvement of the website by observing starting pages, landing pages, ending pages according to user behavior and performed content drilldown to inspect topics of interest to the visitors. Moreover, I analyzed major trends of ad campaigns using Google Ads and determined top keywords, search queries and expenditure. Finally, I provided business suggestions based on acquisition rates from social media networks and types of searches performed by users.
							</div>
						</div>
					</div>
					
					<div class="panel panel-default">
						<div class="panel-heading">
							<h4 class="panel-title">
								<a data-toggle="collapse" data-parent="#accordion" href="#collapseFour" class="collapse_tabs">
									Data Analysis in RStudio - United States Airlines customer satisfaction
									<i class="glyphicon glyphicon-chevron-down" style="float: right;font-size: 13px;"></i> 
								</a>
							</h4>
						</div>
						<div id="collapseFour" class="panel-collapse collapse">
							<div class="panel-body">
								<i class="fa fa-quote-left"></i> Skills acquired: Agile Kanban Methodology, Data analysis, Leadership, Team Management <br>
								Tools: R, Trello, MS PowerPoint, MS Word <br>
								Collaborating with a team of 5 people, I gathered project requirements and summarize project findings as a technology consultant and consistently met deadlines with project team, allocated tasks and followed the agile Kanban methodology using the Trello app. Also, I provided actionable insights by developing a report in MS Word and provided valuable recommendation to the clients using MS PowerPoint. Then, we predicted factors which contribute to high customer satisfaction based on models such as Support Vector Machines, Decision Trees, clustering, classification and Association rule mining using R.
							</div>
						</div>
					</div>
					
					<div class="panel panel-default">
						<div class="panel-heading">
							<h4 class="panel-title">
								<a data-toggle="collapse" data-parent="#accordion" href="#collapseFive" class="collapse_tabs">
									Data Analysis in Excel - House Pricing Analysis
									<i class="glyphicon glyphicon-chevron-down" style="float: right;font-size: 13px;"></i> 
								</a>
							</h4>
						</div>
						<div id="collapseFive" class="panel-collapse collapse">
							<div class="panel-body">
								<i class="fa fa-quote-left"></i> Skills acquired: Data Analysis, Data optimization <br>
								Tools required: MS Excel <br>
								Collaborating with a group of 4 people, I imported real estate data in MS Excel by using PowerQuery and analyzed the dependency of data using PowerPivot, PivotCharts and PowerView. Further, we determined the factors that affect sales depending on prices, size and number of offers using pivot table and charts and predicted the sales patterns by changing the input variables and performing sensitivity analysis.Also, we conducted analysis using correlation and regression techniques to understand relationship and strength of association for data. Finally, we optimized the existing data model and increased sales profit by using scenario manager, goal seek and solver techniques.
							</div>
						</div>
					</div>
					
					<div class="panel panel-default">
						<div class="panel-heading">
							<h4 class="panel-title">
								<a data-toggle="collapse" data-parent="#accordion" href="#collapseSeven" class="collapse_tabs">
								Project Management - RPA at World Hotels for event management
								<i class="glyphicon glyphicon-chevron-down" style="float: right;font-size: 13px;"></i> 
								</a>
							</h4>
						</div>
						<div id="collapseSeven" class="panel-collapse collapse">
							<div class="panel-body">
								<i class="fa fa-quote-left"></i> Skills acquired: Business Analysis, Project management <br>
								Tools used: MS Project, MS Word, MS PowerPoint <br>
								I understood the business need and requirements to share actionable insights. I designed the work breakdown structure (WBS) in MS Project in order to assign and schedule the project tasks to stakeholders and ensured minimum expenditure by estimating the cost of project and allocating budget for various implementation practices.
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</div>