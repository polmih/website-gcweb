---
title: GCWeb, the WET-BOEW Canada.ca theme
altLangPage: accueil.html
dateModified: 2021-11-19
description: "Home page describing all the components of the Canada.ca theme, named GCWeb."
layout: no-container
lang: en
---
<link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.1/css/all.css" integrity="sha384-50oBUHEmvpQ+1lW4y57PTFmhCaXp0ML5d60M1M7uH2+nqUivzIebhndOJK28anvf" crossorigin="anonymous"/>

<div class="container">
	<h1 id="wb-cont" property="name">GCWeb, the WET-BOEW Canada.ca theme</h1>
	<div class="row">
		<div class="col-md-7 col-lg-8">
			<p>The page templates and design patterns below comprise a reference implementation of the <a href="https://design.canada.ca">Canada.ca design system</a>, including the mandatory requirement of the Content and Information Architecture (C&amp;IA) Specification. Government of Canada departments and agencies can contribute additional patterns and templates via <a href="https://github.com/wet-boew/GCWeb">GCWeb github repository</a>.</p>
		</div>
		<div class="col-xs-12 col-md-auto pull-right">
			<p><a href="https://github.com/wet-boew/GCWeb/archive/v9.5.0.zip" class="btn btn-primary">Download GCWeb theme <strong>v9.5.0</strong></a><br>
				<small>(<time>2021-08-06</time> - <a href="https://github.com/wet-boew/gcweb/releases/tag/v9.5.0">Release notes</a>)</small></p>
		</div>
	</div>
</div>
<div class="container-fluid wb-inview show-none bar-demo" data-inview="nav-menu">
	<div class="row">
		<nav class="well well-lg mrgn-tp-md">
			<div class="container">
				<h2 class="mrgn-tp-0">Get started</h2>
				<ul class="list-unstyled colcount-md-3">
					<li><a href="#components"><span aria-hidden="true" class="fas fa-cube mrgn-rght-md"></span>Components</a></li>
					<li><a href="#templates"><span aria-hidden="true" class="fas fa-table mrgn-rght-md"></span>Templates</a></li>
					<li><a href="#experiment"><span aria-hidden="true" class="fas fa-puzzle-piece mrgn-rght-md"></span>Méli-mélo and thematics</a></li>
					<li><a href="#sitesglobal"><span aria-hidden="true" class="fas fa-globe mrgn-rght-md"></span>Sites and global functionality</a></li>
					<li><a href="#other"><span aria-hidden="true" class="fas fa-info-circle mrgn-rght-md"></span>Other documentation</a></li>
					<li><a href="#developping-for-gcweb"><span aria-hidden="true" class="fas fa-code mrgn-rght-md"></span>Developing for GCWeb</a></li>
				</ul>
			</div>
		</nav>
	</div>
</div>
<section id="nav-menu" class="wb-overlay modal-content overlay-def wb-bar-t hidden-xs" aria-hidden="true">
<header class="pull-left">
	<h2 class="modal-title">Get started</h2>
</header>
<ul class="pull-left list-inline mrgn-lft-md mrgn-tp-sm">
	<li><a href="#components" class="btn btn-link text-white"><span aria-hidden="true" class="fas fa-cube mrgn-rght-md"></span>Components</a></li>
	<li class="mrgn-lft-md"><a href="#templates" class="btn btn-link text-white"><span aria-hidden="true" class="fas fa-table mrgn-rght-md"></span>Templates</a></li>
	<li class="mrgn-lft-md"><a href="#méli-mélo" class="btn btn-link text-white"><span aria-hidden="true" class="fas fa-puzzle-piece mrgn-rght-md"></span>Méli-mélo and thematics</a></li>
	<li class="mrgn-lft-md"><a href="#sitesglobal" class="btn btn-link text-white"><span aria-hidden="true" class="fas fa-globe mrgn-rght-md"></span>Sites and global</a></li>
	<li class="mrgn-lft-md"><a href="#other" class="btn btn-link text-white"><span aria-hidden="true" class="fas fa-info-circle mrgn-rght-md"></span>Other</a></li>
	<li class="mrgn-lft-md"><a href="#developping-for-gcweb" class="btn btn-link text-white"><span aria-hidden="true" class="fas fa-code mrgn-rght-md"></span>Developing for GCWeb</a></li>
</ul>
</section>
<div class="container">
<p><small>Found an C&amp;IA implementation issue or you want to contribute at their development, let us know by submiting <a href="https://github.com/wet-boew/GCWeb/issues/new?title=C&amp;IA%20implementation%20error:%20">GCweb issue</a>, sending <a href="https://github.com/wet-boew/GCWeb/pulls">pull request</a> or by participating at one of our <a href="https://wet-boew.github.io/wet-boew-documentation/index-en.html#wet-boew-code-sprint">WET-BOEW weekly Tuesday code sprint</a>.</small></p>

<p>The following status was not transposed yet with the repository structure reorg:</p>
<details>
	<summary>Meaning of statuses</summary>
	<dl class="dl-horizontal mrgn-bttm-0">
		<dt><span class="label label-success">Stable</span></dt>
		<dd>Meet the latest published specification.</dd>
		<dt><span class="label label-warning">Provisional</span></dt>
		<dd>Use as your own risks.</dd>
		<!--<dt><span class="label label-success">Up to spec</span></dt>
		<dd>Meet the latest published C&amp;IA specification.</dd>
		<dt><span class="label label-info">Informational</span></dt>
		<dd>It's for your information. It's complete and suggestive but not defined by and from a specification yet.</dd>
		<dt><span class="label label-info">Need to revalidate</span></dt>
		<dd>Was meeting the preceding published specification, but it need to be manually revalidated to ensure it continues to meet the latest published specification.</dd>
		<dt><span class="label label-warning">Partial</span></dt>
		<dd>Partially up to spec or partially stable in order to meet other core web standards such WCAG 2.0 Level AA.</dd>
		<dt><span class="label label-warning">Outdated</span></dt>
		<dd>Don't meet the latest specification but met a previous version. It requires updates.</dd>
		<dt><span class="label label-default">Backlog</span></dt>
		<dd>Need to be developped.</dd>
		<dt><span class="label label-danger">Incomplete</span></dt>
		<dd>Incomplete because it don't fully meet all the specification yet. Still need developpement work.</dd>
		<dt><span class="label label-danger">Deprecated</span></dt>
		<dd>Do not use because it's deprecated, but listed here for your information.</dd>-->
	</dl>
</details>

<h2 id="components">Components</h2>

<p>List of components here.</p>

<h2 id="templates">Templates</h2>
<ul class="row list-unstyled wb-eqht">

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md">Advanced Service - Probably deprecated <span class="label label-default small"><span class="wb-inv">State: </span>Stable</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/advancedservice/index-en.html" lang="en" hreflang="en">[Service name] - 1. [Step / section page name]</a></li>
				
			
				
				<li><a href="templates/advancedservice/page2-en.html" lang="en" hreflang="en">[Service name] - 2. [Step / section page name]</a></li>
				
			
				
				<li><a href="templates/advancedservice/page3-en.html" lang="en" hreflang="en">[Service name] - 3. [Step / section page name]</a></li>
				
			
				
				<li><a href="templates/advancedservice/page4-en.html" lang="en" hreflang="en">[Service name] - 4. [Step / section page name]</a></li>
				
			
				
				<li><a href="templates/advancedservice/page5-en.html" lang="en" hreflang="en">[Service name] - 5. [Step / section page name]</a></li>
				
			
				
				<li><a href="templates/advancedservice/page6-en.html" lang="en" hreflang="en">[Service name] - 6. [Step / section page name]</a></li>
			</ul>
			
			</details>
	</ul>
	</div></li>

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md"><a href="templates/campaign/api.html" lang="en" hreflang="en">Campaign name</a> <span class="label label-default small"><span class="wb-inv">State: </span>Stable</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/campaign/campaign-en.html" lang="en" hreflang="en">Campaign name</a></li>
				
			
				
				<li><a href="templates/campaign/campaign2-en.html" lang="en" hreflang="en">Campaign name 2</a></li>
			</ul>
			
			</details>

	</ul>
	</div></li>

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md"><a href="templates/home/api.html" lang="en" hreflang="en">Home</a> <span class="label label-default small"><span class="wb-inv">State: </span>Stable</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/home/home-en.html" lang="en" hreflang="en">Home - Canada.ca</a></li>
			</ul>
			
			</details>
	</ul>
	</div></li>

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md">Other template <span class="label label-default small"><span class="wb-inv">State: </span>Stable</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/content-en.html" lang="en" hreflang="en">Content page</a></li>
				
			
				
				<li><a href="templates/content-fluid-en.html" lang="en" hreflang="en">Fluid content page</a></li>
				
			
				
				<li><a href="templates/content-limit-en.html" lang="en" hreflang="en">Content page - Limited width content</a></li>
				
			
				
				<li><a href="templates/content-gcweb-4-0-29-font-style-en.html" lang="en" hreflang="en">Content page - GCWeb 4.0.29 font stylee</a></li>
				
			
				
				<li><a href="templates/content-signedoff-en.html" lang="en" hreflang="en">Content page - Signed Off</a></li>
				
			
				
				<li><a href="templates/content-signedon-en.html" lang="en" hreflang="en">Content page - Signed On</a></li>
				
			
				
				<li><a href="templates/widgets-en.html" lang="en" hreflang="en">Stay connected</a></li>
				
			
				
				<li><a href="templates/theme-en.html" lang="en" hreflang="en">[Theme title]</a></li>
				
			
				
				<li><a href="templates/dept-en.html" lang="en" hreflang="en">Departments and agencies</a></li>
				
			
				
				<li><a href="templates/event-en.html" lang="en" hreflang="en">Promotional events page (Campaign?)</a></li>
				
			
				
				<li><a href="templates/feedback-en.html" lang="en" hreflang="en">Feedback form</a></li>
				
			
				
				<li><a href="templates/gc-audience-en.html" lang="en" hreflang="en">[Audience name]</a></li>
				
			
				
				<li><a href="templates/service-en.html" lang="en" hreflang="en">Service initiation - Might deprecated</a></li>
			</ul>
			
			</details>
	</ul>
	</div></li>

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md"><a href="templates/index/api.html" lang="en" hreflang="en">Index</a> <span class="label label-default small"><span class="wb-inv">State: </span>Stable</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/index/longindex-en.html" lang="en" hreflang="en">[Long index page]</a></li>
			</ul>
			
			</details>
	</ul>
	</div></li>

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md">Institutional profile <span class="label label-default small"><span class="wb-inv">State: </span>Stable</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/institutional/institution-en.html" lang="en" hreflang="en">[Institution Name]</a></li>
				
			
				
				<li><a href="templates/institutional/institution-landing-en.html" lang="en" hreflang="en">[Institution Name] - landing page (provisional)</a></li>
				
			
				
				<li><a href="templates/institutional/institution-contact-en.html" lang="en" hreflang="en">Contact [Institution name]</a></li>
				
			
				
				<li><a href="templates/institutional/institutional-service-performance-en.html" lang="en" hreflang="en">[Institution] service performance reporting for fiscal year 2015 to 2016</a></li>
				
			
				
				<li><a href="templates/institutional/institution-arms-en.html" lang="en" hreflang="en">arm’s length - [Institution Name]</a></li>
			</ul>
			
			</details>
	</ul>
	</div></li>

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md">Laws and regulations pages <span class="label label-default small"><span class="wb-inv">State: </span>Stable</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/legislation/act-en.html" lang="en" hreflang="en">[Act name] <small>([NN-XX])</small></a></li>
				
			
				
				<li><a href="templates/legislation/regulations-en.html" lang="en" hreflang="en">[Regulation name] <small>([NN-XX])</small></a></li>
			</ul>
			
			</details>
	</ul>
	</div></li>

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md">Local navigation <span class="label label-default small"><span class="wb-inv">State: </span>Stable</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/localnav/index-en.html" lang="en" hreflang="en">[Topic - Local navigation]</a></li>
				
			
				
				<li><a href="templates/localnav/task1/index-en.html" lang="en" hreflang="en">Task 1</a></li>
				
			
				
				<li><a href="templates/localnav/task1/task1/index-en.html" lang="en" hreflang="en">Sub task 1</a></li>
				
			
				
				<li><a href="templates/localnav/task1/task2/index-en.html" lang="en" hreflang="en">Sub task 2</a></li>
				
			
				
				<li><a href="templates/localnav/task1/task3/index-en.html" lang="en" hreflang="en">Sub task 3</a></li>
				
			
				
				<li><a href="templates/localnav/task1/task4/index-en.html" lang="en" hreflang="en">Sub task 4</a></li>
				
			
				
				<li><a href="templates/localnav/task1/task5/index-en.html" lang="en" hreflang="en">Sub task 5</a></li>
				
			
				
				<li><a href="templates/localnav/task1/task6/index-en.html" lang="en" hreflang="en">Sub task 6</a></li>
				
			
				
				<li><a href="templates/localnav/task1/task7/index-en.html" lang="en" hreflang="en">Sub task 7</a></li>
				
			
				
				<li><a href="templates/localnav/task2/index-en.html" lang="en" hreflang="en">Task 2</a></li>
				
			
				
				<li><a href="templates/localnav/task3/index-en.html" lang="en" hreflang="en">Task 3</a></li>
				
			
				
				<li><a href="templates/localnav/task3/task1/index-en.html" lang="en" hreflang="en">Sub task 1</a></li>
				
			
				
				<li><a href="templates/localnav/task3/task2/index-en.html" lang="en" hreflang="en">Sub task 2</a></li>
				
			
				
				<li><a href="templates/localnav/task3/task2/task1/index-en.html" lang="en" hreflang="en">Sub sub task 1</a></li>
				
			
				
				<li><a href="templates/localnav/task3/task2/task2/index-en.html" lang="en" hreflang="en">Sub sub task 2</a></li>
				
			
				
				<li><a href="templates/localnav/task3/task3/index-en.html" lang="en" hreflang="en">Sub task 3</a></li>
				
			
				
				<li><a href="templates/localnav/task4/index-en.html" lang="en" hreflang="en">Task 4</a></li>
			</ul>
			
			</details>
	</ul>
	</div></li>

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md"><a href="templates/ministerial/ministerial-doc-en.html" lang="en" hreflang="en">Ministerial profile</a> <span class="label label-default small"><span class="wb-inv">State: </span>Stable</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/ministerial/ministerial-en.html" lang="en" hreflang="en">Ministerial profile</a></li>
				
			
				
				<li><a href="templates/ministerial/ministerial-reduced-en.html" lang="en" hreflang="en">Ministerial profile - swearing-in day</a></li>
			</ul>
			
			</details>
	</ul>
	</div></li>

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md">News <span class="label label-default small"><span class="wb-inv">State: </span>Stable</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/news/news-en.html" lang="en" hreflang="en">News</a></li>
			</ul>	
			
			</details>
	</ul>
	</div></li>

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md">Organizational profile <span class="label label-default small"><span class="wb-inv">State: </span>Stable</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/organizational/organizational-en.html" lang="en" hreflang="en">[Organization Name]</a></li>
				
			
				
				<li><a href="templates/organizational/organizational-arms-en.html" lang="en" hreflang="en">arm’s length - [Organization Name]</a></li>
			</ul>
			
			</details>
	</ul>
	</div></li>

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md"><a href="templates/search/api.html" lang="en" hreflang="en">Search results</a> <span class="label label-default small"><span class="wb-inv">State: </span>Stable</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/search/results-en.html" lang="en" hreflang="en">Search results</a></li>
				
			
				
				<li><a href="templates/search/results-filters-en.html" lang="en" hreflang="en">Search facets/filters results</a></li>
				
			
				
				<li><a href="templates/search/results-contextual-en.html" lang="en" hreflang="en">Contextual</a></li>
			</ul>
			
			</details>
	</ul>
	</div></li>

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md">Server error message <span class="label label-default small"><span class="wb-inv">State: </span>Stable</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/servermessage/404-en.html" lang="en" hreflang="en">We couldn't find that Web page (Error 404) - Canada.ca theme</a></li>
				
			
				
				<li><a href="templates/servermessage/404-en-fr.html" lang="en" hreflang="en">We couldn't find that Web page (Error 404) - Canada.ca theme / Nous ne pouvons trouver cette page Web (Erreur 404) - Thème Canada.ca</a></li>
				
			
				
				<li><a href="templates/servermessage/servermessage-en.html" lang="en" hreflang="en">Message title - Canada.ca theme</a></li>
				
			
				
				<li><a href="templates/servermessage/servermessage-en-fr.html" lang="en" hreflang="en">Message title - Canada.ca theme / Titre du message - Thème Canada.ca</a></li>
			</ul>
			
			</details>
	</ul>
	</div></li>

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md">Splash page - Canada.ca <span class="label label-default small"><span class="wb-inv">State: </span>Stable</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/splash/splashpage.html" lang="en" hreflang="en">Splash page example</a></li>
			</ul>
			
			</details>
	</ul>
	</div></li>

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md">Thematic <span class="label label-default small"><span class="wb-inv">State: </span>Provisional</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/thematic/pink-day-en.html" lang="en" hreflang="en">Pink Day</a></li>
				
			
				
				<li><a href="templates/thematic/dark-theme-en.html" lang="en" hreflang="en">Dark theme</a></li>
			</ul>
			
			</details>
	</ul>
	</div></li>

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md">Beta - Theme, Topic <span class="label label-default small"><span class="wb-inv">State: </span>Provisional</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/theme-topic/theme-topic-en.html" lang="en" hreflang="en">[Theme - Topic title]</a></li>
			</ul>
			
			</details>
	</ul>
	</div></li>

	
	<li class="col-md-6 mrgn-bttm-md">
		<div class="brdr-tp brdr-rght brdr-bttm brdr-lft hght-inhrt">
			<h3 class="mrgn-tp-md mrgn-rght-md mrgn-bttm-md mrgn-lft-md">Topic <span class="label label-default small"><span class="wb-inv">State: </span>Stable</span></h3>
			<ul class="list-unstyled mrgn-rght-md mrgn-bttm-md mrgn-lft-md">
	
		
		<p>Short description of the template</p>
	<details class="mrgn-tp-lg"><summary>Examples</summary>
			<ul>
			
			
				
				<li><a href="templates/topic/topic-en.html" lang="en" hreflang="en">[Topic title]</a></li>
				
			
				
				<li><a href="templates/topic/topic-testcase-1-en.html" lang="en" hreflang="en">[Topic title, test case 1]</a></li>
			</ul>
			
			</details>
	</ul>
	</div></li>

</ul>

</div>
<div class="container-fluid">
	<div class="row">
		<div class="well well-lg mrgn-tp-md bg-gctheme text-white">
			<div class="container mrgn-bttm-lg">
				<h2 id="experiment" class="mrgn-bttm-0">Special features</h2>
					<div class="row">
					    <div class="col-md-6">
					    	<h3 id="méli-mélo">Méli-mélo</h3>
						<p>This is the experimentation hub you have been waiting for! Méli-mélos allow you to bring in some awesome new stuff.</p>
						<p class="mrgn-tp-lg"><a href="méli-mélo/méli-mélo-en.html" class="btn btn-default btn-lg">Learn more<span class="wb-inv"> about méli-mélo</span></a></p>
					    </div>
					    <div class="col-md-6">
						<h3 id="thematics">Promotional thematics</h3><p>This is the experimentation hub you have been waiting for! Méli-mélos allow you to bring in some awesome new stuff.</p>
						<p class="mrgn-tp-lg"><a href="th%C3%A9matique/gc-th%C3%A9matique-en.html" class="btn btn-default btn-lg">Learn more<span class="wb-inv"> about promotional thematics</span></a></p>
				</div>
			</div>
        	</div>
        </div>
    </div>
</div>
<div class="container">

<h2 id="sitesglobal">Sites and global functionality</h2>
<ul>

	
	<li>Site wide demoed feature (État: Stable)
	<ul>
	
		
		<li>Examples
			<ul>
			
			
				
				<li><a href="sites/archived/archived-en.html" lang="en" hreflang="en">Archived - Content page</a></li>
				
			
			</ul>
		</li>
	
	</ul></li>

	
	<li>Breadcrumbs (État: Stable)
	<ul>
	
		
		<li>Documentations
			<ul>
			
			
				
				<li><a href="sites/breadcrumbs/breadcrumbs-en.html" lang="en" hreflang="en">Breadcrumbs</a></li>
				
			
			</ul>
		</li>
	
	</ul></li>

	
	<li>Helpers (État: Stable)
	<ul>
	
		
		<li>Documentations
			<ul>
			
			
				
				<li><a href="sites/helpers/colour-en.html" lang="en" hreflang="en">Colour</a></li>
				
			
			</ul>
		</li>
	
	</ul></li>

</ul>

<h2 id="other">Other documentation</h2>

<h3>WET-BOEW feature demos styled with Canada.ca theme</h3>
<p><a href="/gcweb-compiled-demos/index.html#wet-boew">WET-BOEW feature overview</a></p>

<h3 id="gcweb-project-documentation">GCWeb project documentation</h3>

<ul>
  <li><a href="/GCWeb/docs/">GCWeb theme - Meta information</a></li>
  <li><a href="/GCWeb/docs/implementing.html">Quick implementation guide - GCWeb theme</a></li>
  <li><a href="/GCWeb/docs/v5-migration.html">Migration instruction - GCWeb theme V5</a></li>
  <li><a href="/GCWeb/docs/GCWeb-en.html">Archived - Documentation - GCWeb English</a></li>
  <li><a href="/GCWeb/docs/release/index-en.html">Archived - Releases English</a></li>
  <li><a href="/GCWeb/docs/static-header-footer/bootstrap-3.html">Skeleton - Static header/footer - Bootstrap 3</a></li>
  <li><a href="/GCWeb/docs/static-header-footer/bootstrap-4.html">Prototype skeleton - Static header/footer - Bootstrap 4</a></li>
</ul>

<p>Evaluations and reports</p>

<ul>
  <li><a href="/GCWeb/docs/evaluation-report/1-accessibility.html">1 - Accessibility assessment as 2018-11-14</a></li>
  <li><a href="/GCWeb/docs/evaluation-report/2-wetplugin-gcweb2.html">2 - Regression user acceptance testing as 2018-11-16</a></li>
</ul>

<h2 id="developping-for-gcweb"><span aria-hidden="true" class="fas fa-code mrgn-rght-md"></span>Developping for GCWeb</h2>

<p>Install NodeJS</p>

<h3 id="building-gcweb">Building GCweb</h3>

<ul>
  <li>Build a local development version: <code class="language-plaintext highlighter-rouge">grunt</code> or <code class="language-plaintext highlighter-rouge">grunt debug</code></li>
  <li>Run code quality check: <code class="language-plaintext highlighter-rouge">grunt test</code></li>
  <li>Build production files: <code class="language-plaintext highlighter-rouge">grunt dist</code></li>
  <li>Compile and assemble méli-mélo:
	<ul>
	  <li>Run local: <code class="language-plaintext highlighter-rouge">grunt méli-mélo</code></li>
	  <li>Run from compiled dist: <code class="language-plaintext highlighter-rouge">grunt méli-mélo-runLocal</code></li>
	  <li>Run from wet-boew sites : <code class="language-plaintext highlighter-rouge">grunt méli-mélo-remote</code></li>
	</ul>
  </li>
  <li>Regenerate site web content: <code class="language-plaintext highlighter-rouge">grunt site-contents</code>
	<ul>
	  <li><code class="language-plaintext highlighter-rouge">_data/components.json</code></li>
	  <li><code class="language-plaintext highlighter-rouge">_data/sites.json</code></li>
	  <li><code class="language-plaintext highlighter-rouge">_data/templates.json</code></li>
	  <li><code class="language-plaintext highlighter-rouge">_wetboew-demos/**</code></li>
	</ul>
  </li>
</ul>

<h3 id="run-gcweb-wetsite-locally">Run GCWeb wetsite locally</h3>

<p>Ensure that you have builded GCWeb first</p>

<p>After your are running docking container or the docker composer you will be able to access your local website at: <code class="language-plaintext highlighter-rouge">http://localhost:4000</code></p>

<p>Build Dockerfile locally</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>docker build -t jekyll-with-env-options .
</code></pre></div></div>

<p>Run your image</p>
<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>grunt debug

docker run -it --rm -v "$PWD":/usr/src/app -p "4000:4000" --env JEKYLL_OPTIONS='--config _config.yml,_localJekyll.yml' jekyll-with-env-options
</code></pre></div></div>

<h4 id="alternative-with-docker-compose">alternative with docker-compose</h4>

<p>This version leverage the remote theme wet-beoew/gcweb-jekyll. This equivalent if you run with gh-pages through your own GCWeb repository.</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>docker-compose up
</code></pre></div></div>

<h3 id="run-the-continous-integration-and-deployment-script-locally">Run the continous integration and deployment script locally</h3>

<p>Install ACT - <a href="https://github.com/nektos/act">https://github.com/nektos/act</a></p>

<p>Github fork needed:</p>

<ul>
  <li><a href="https://github.com/wet-boew/gcweb">wet-boew/gcweb</a></li>
  <li><a href="https://github.com/wet-boew/gcweb-jekyll">wet-boew/gcweb-jekyll</a></li>
  <li><a href="https://github.com/wet-boew/gcweb-compiled-demos">wet-boew/gcweb-compiled-demos</a></li>
  <li><a href="https://github.com/wet-boew/themes-dist">wet-boew/themes-dist</a></li>
  <li><a href="https://github.com/wet-boew/themes-cdn">wet-boew/themes-cdn</a></li>
</ul>

<p>Run the continuous deployment script</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>act -f deploy-gcweb -s my_token=&lt;XXXXXXXXXXXXXX&gt; -s my_username="&lt;GITHUB USERNAME&gt;" - my_email="&lt;GITHUB HANDLE&gt;@users.noreply.github.com" -a &lt;GITHUB HANDLE&gt;
</code></pre></div></div>

<p>Where:</p>
<ul>
  <li><code class="language-plaintext highlighter-rouge">&lt;GITHUB USERNAME&gt;</code>: Your name, like “John Doe”</li>
  <li><code class="language-plaintext highlighter-rouge">&lt;GITHUB HANDLE&gt;</code>: Your github id</li>
  <li><code class="language-plaintext highlighter-rouge">&lt;XXXXXXXXXXXXXX&gt;</code>: Your personal access token with access to public repository</li>
</ul>

<h3 id="refresh-your-github-pages-with-the-latest-theme-changes">Refresh your github pages with the latest theme changes</h3>

<p>You can make a commit to your site and it will get regenerated with the latest version of the jekyll theme. Alternatively, the following curl command will told github to regenerate your site.</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>curl -u &lt;GITHUB HANDLE&gt;:&lt;XXXXXXXXXXXXXX&gt; -X POST https://api.github.com/repos/&lt;GITHUB HANDLE&gt;/&lt;GITHUB REPOSITORY&gt;/pages/builds
</code></pre></div></div>

<p>Where:</p>
<ul>
  <li><code class="language-plaintext highlighter-rouge">&lt;GITHUB HANDLE&gt;</code>: Your github id</li>
  <li><code class="language-plaintext highlighter-rouge">&lt;XXXXXXXXXXXXXX&gt;</code>: Your personal access token with access to public repository</li>
  <li><code class="language-plaintext highlighter-rouge">&lt;GITHUB REPOSITORY&gt;</code>: Your web site github repository, like “jekyll-website”</li>
</ul>

<p>Note: A manual update is required if you have specified a version for your jekyll remote theme in your <code class="language-plaintext highlighter-rouge">config.yml</code> file.</p>
	</div>
