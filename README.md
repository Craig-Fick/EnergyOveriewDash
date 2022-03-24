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
<iframe src="https://public.tableau.com/views/EnergyOverviewDash/Dashboard1?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link"></iframe>
<iframe src="https://public.tableau.com/views/EnergyOverviewDash/Dashboard1?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link" width = '650' height = '450'></iframe>
