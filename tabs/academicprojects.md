---
title: Academic Projects

# The About page
# v2.0
# https://github.com/cotes2020/jekyll-theme-chirpy
# © 2017-2019 Cotes Chung
# MIT License
---
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
.accordion {
  background-color: #eee;
  color: #444;
  cursor: pointer;
  padding: 18px;
  width: 100%;
  border: none;
  text-align: left;
  outline: none;
  font-size: 15px;
  transition: 0.4s;
}

.active, .accordion:hover {
  background-color: #ccc;
}

.accordion:after {
  content: '\002B';
  color: #777;
  font-weight: bold;
  float: right;
  margin-left: 5px;
}

.active:after {
  content: "\2212";
}

.panel {
  padding: 0 18px;
  background-color: white;
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.2s ease-out;
}
</style>
</head>
<body>

<button class="accordion">Data Analysis on Loan Data using R and Tableau</button>
<div class="panel">
  <p>For this project, I started off with cleaning data and selecting important variables to ensure meaningful and actionable insights are drawn using data models in R. 
  Then, I applied data analytics algorithms like decision tree, Naïve Bayes and kNN classification algorithm to develop strategic initiatives. 
  Moreover, I built machine learning algorithms to predict loan defaults based on various factors by using random forests and SVMs at an accuracy of 93% and 98% respectively. 
  Finally, I built customized, interactive reports and dashboards using Tableau to help businesses gain insights about loan defaults in the USA.</p>
</div>

<button class="accordion">Database Management for Developing a Health Care Portal using SQL, MS Access, MS Visio and VBA</button>
<div class="panel">
  <p>In this project, the team and I implemented a database management system for a health care portal. 
  Here, our main task was to communicate with users and identify their requirements and translate them into robust functional requirements. 
  We documented these requirements and established business rules for creating the Entity-Relation Diagram using MS Access and MS Visio. 
  After reaching common ground with the user about the business rules, we then implemented the same design in SQL Server Management Studio and used MS Access to build forms and dashboards. 
  With this system in place, we are looking to decrease human intervention, and thereby errors, by automating the appointment booking to bill generation process.</p>
</div>

<button class="accordion">Development of Data Warehouse for Local Grocery Chain using SQL, SSIS, SSAS and Visual Studio</button>
<div class="panel">
  <p>For this Business Intelligence venture, I designed and engineered a data warehouse for a local grocery chain to analyze factors such as sales, inventory, customer satisfaction. 
  To accomplish this, I developed datamarts using dimensional modeling worksheets to load data into a centralized database from different data sources. 
  Furthermore, I built MOLAP to expedite the process of generating reports for executives for exploratory data analysis and root cause analysis.</p>
</div>

<button class="accordion">Data Analysis on Customer Satisfaction Survey</button>
<div class="panel">
  <p>During this project, I collaborated in a group of 4 to perform exploratory and explanatory data analysis on the customer satisfaction survey of several airlines to find critical business insights on how to improve customer satisfaction. 
  The team and I started with acquiring data and performing transformations such as cleaning and munging to ensure that the data is of quality. 
  Then, I built models like Support Vector Machine, Association Rule Mining and created impactful visualizations to validate the analysis. 
  Furthermore, the team and I developed a report which consisted of analysis and recommendations to the client team on the same.</p>
</div>

<button class="accordion">Data Analysis for House Sales using Advanced MS Excel</button>
<div class="panel">
  <p>For this analysis, I investigated factors that influence the price of houses and used them to predict sales patterns by using advanced Excel functions. 
  This was accomplished by analyzing the dependency of data by importing data in MS Excel using PowerQuery and utilizing functions like PowerPivot, PowerView. 
  Then, I explored sales depending on factors like prices, size, number of offers using correlation and regression techniques. 
  Furthermore, I created Excel models using scenario manager, goal seek and solver to optimize business processes to increase revenue. 
  Finally, I developed impactful and enriching dashboards and reports using Power BI and MS Excel to help the business gain actionable insights.</p>
</div>

<button class="accordion">Business Analytics using Google Analytics</button>
<div class="panel">
  <p>With the use of Google Analytics, I was able to track the demographics of the visitors and the devices used to connect to my website which helped me understand the current audience of the website. 
  This helped me to give ad suggestions and content suggestions to the business to target these visitors. 
  I also planned and managed A/B tests to drive core insights from available data to drive improvements and recommendations. 
  I could also suggest improvements in the website to the business by inspecting parameters such as Page Views, Sessions, Avg. Session Duration and Bounce Rate. 
  I also helped business understand the key interests of the visitors by performing content drilldown technique. 
  Furthermore, I analyzed major trends of ad campaigns using Google Ads to determine top keywords, search queries, and expenditure of these ad campaigns. 
  Finally, I provided the business with suggestions based on acquisition rates from social media networks and types of searches performed by users.</p>
</div>

<button class="accordion">Robotic Process Automation at World Hotels for Event Management</button>
<div class="panel">
  <p>In this project, I had to coordinate and lead with teams to deploy RPA software prototype to automate numerous steps involved in event management for hospitality customers. 
  I continuously communicated with the users to translate user case stories and ideas into comprehensive business requirements. 
  Furthermore, I reviewed business requirements according to their priorities and analyzed options, risks, and costs via MS Project. 
  I was also responsible for creating an executive overview presentation via MS PowerPoint detailing the benefits and use of RPA to senior executives of the client organization. 
  During this project I led project teams, internal and external, to achieve project defined milestones and deliverables.</p>
</div>

<button class="accordion">Risk Analysis in a Book Store</button>
<div class="panel">
  <p>During this project, I performed a risk analysis by collaborating with various multi-functional teams in a book store to determine risks affecting regular operations. 
  To ensure that risks are addressed appropriately I complied a risk register by researching company, its infrastructure and analyzing past incidents along with charting a risk map. 
  Additionally, I collaborated with the managers and recommended and implemented contingency and disaster recovery plans to minimize book store losses and ensure asset protection.
</p>
</div>

<script>
var acc = document.getElementsByClassName("accordion");
var i;

for (i = 0; i < acc.length; i++) {
  acc[i].addEventListener("click", function() {
    this.classList.toggle("active");
    var panel = this.nextElementSibling;
    if (panel.style.maxHeight) {
      panel.style.maxHeight = null;
    } else {
      panel.style.maxHeight = panel.scrollHeight + "px";
    } 
  });
}
</script>

</body>
</html>