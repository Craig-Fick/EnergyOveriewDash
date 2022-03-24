# EnergyOveriewDash
This project uses python to scrape energy data hourly in the U.S. and then uploads it to AWS S3 where it is then connected live to Tableau.

Steps:
1. Create AWS account.
2. Create AWS bucket in S3 and get key id and secret key.
3. Run Python scraping script to establish and upload data to AWS.
4. Open AWS Athena and use Query language to create database, data table, and data view.
5. Connect Tableau to Athena data with Athena key id and secret key.
6. Build dashboard


The data is collected from:
https://www.eia.gov/electricity/gridmonitor/dashboard/electric_overview/US48/US48

The dashboard created:
<div class='tableauPlaceholder' id='viz1648157558145' style='position: relative'><noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;En&#47;EnergyOverviewDash&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='EnergyOverviewDash&#47;Dashboard1' /><param name='tabs' value='yes' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;En&#47;EnergyOverviewDash&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object></div>               
<script type='text/javascript'> var divElement = document.getElementById('viz1648157558145'); var vizElement = divElement.getElementsByTagName('object')[0]; if ( divElement.offsetWidth > 800 ) { vizElement.style.minWidth='1000px';vizElement.style.maxWidth='100%';vizElement.style.minHeight='850px';vizElement.style.maxHeight=(divElement.offsetWidth*0.75)+'px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.minWidth='1000px';vizElement.style.maxWidth='100%';vizElement.style.minHeight='850px';vizElement.style.maxHeight=(divElement.offsetWidth*0.75)+'px';} else { vizElement.style.width='100%';vizElement.style.minHeight='1100px';vizElement.style.maxHeight=(divElement.offsetWidth*1.77)+'px';} var scriptElement = document.createElement('script'); scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js'; vizElement.parentNode.insertBefore(scriptElement, vizElement); </script>
