---
title: "HBML - Resources"
layout: gridlay
excerpt: "Resources"
sitemap: false
permalink: /resources
---

<style>
.well {
  height: 300px; /* Adjust the height as needed */
  overflow: auto; /* Add scroll if content exceeds the height */

  .clearfix::after {
  content: "";
  display: table;
  clear: both;
}
}
</style>

# Resources
This page contains links to code or other useful materials we developed. 

## Code
<div>
<div class="col-sm-6 clearfix">
 <div class="well">
<pubtit><a href="{{ site.baseurl }}/downloads/seecog_poster_aes_2020.pdf">SEECOG</a></pubtit>  
<img src="{{ site.url }}{{ site.baseurl }}/images/research/Seecog.png" class="img-responsive" width="50%" style="float: left" />
  <p><em>Viewing and intuitive interaction with multimodal data from intracranial patients is
challenging. We developed a browser based viewer that:
• Does not require installation of additional software
• Has dynamic 3D rendering for easy adjustments of views
• Runs locally (no need for internet, no need to upload sensitive data to a server)
• Works on every OS
• Does not require technical knowledge</em></p>
 </div>
</div>

<div class="col-sm-6 clearfix">
 <div class="well">
 <pubtit><a href="http://ielvis.pbworks.com/w/page/116347253/FrontPage" target="_blank">iElvis</a></pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/iElvis_logo.png" class="img-responsive" width="50%" style="float: left" />
  <p><em>Accurate intracranial electrode localization and visualization is a pre-requisite for all iEEG research. iElvis is a toolbox that helps with both those aspects. 
    Groppe, DM. et al. J Neurosci Meth 281, 40–48 (2017).
  </em></p>
 </div>
</div>

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit><a href="https://github.com/IEEG/iEEG2NWB" target="_blank">iEEG2NWB</a></pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/logos/NWB_logo.png" class="img-responsive" width="50%" style="float: left" />
  <p><em><a href="https://www.nwb.org" target="_blank">Neurodata without Borders (NWB)</a> is a newly developed standard to save neurophysiology data. We developed Python code to import our iEEG data, other neurophysiological signals, and meta-data from command line or via a GUI. We tried to make it as useable for other labs as possible. Try it out and please let us know if you have suggestions! 
  Thank you to the Kavli Foundation's Seed Grant to Stephan, which helped developing this!
  </em></p>
 </div>
</div>


<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit><a href="https://github.com/IEEG/" target="_blank">EPIPE</a></pubtit>
  <p><em> Our iEEG preprocessing and analysis code. (We're currently cleaning it up for you. Stay tuned.)
  </em></p>
 </div>
</div>

<div class="clearfix"></div>

<hr> <!-- Add a horizontal rule here -->

## Data
  <p>We are committed to sharing our data in NWB format and are in the process of converting our old and new data. We will list all the data we share here. Stay tuned.</p>

<ul>
    <li><a href="https://osf.io/9bzx8/?view_only=ed6f1eba830840cb9921458490b3c362" target="_blank"> Code and data</a> for the paper <i>Intracranial electroencephalography reveals effector-independent evidence accumulation dynamics in multiple human brain regions.</i>. Gherman et al. Nat. Hum. Behav. 8, 758–770 (2024). (stay tuned for an NWB version)
    <li>...in process. For now check our the links to code and data on our publications.
</ul>


{% comment %}
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/DSC_0696.jpg" width="95%">
</figure>
{% endcomment %}
