# POPE

This repository contains the dataset collected within the scope of my master's thesis and the results of the classification process. 

It is organized in two main folders:
- The [dataset](./dataset) folder contains all the data related to the collection made, which was later used in the prompts made for the LLM models. It includes all the information without further transformations and the modified versions. 
  - The [categories](./dataset/raw_data/categories.csv) file contains a list of all the categories of websites used to collect data from and each corresponding URL to the category metadata and list of websites.
  - The [websites](./dataset/raw_data/websites.csv) file contains the set of all top 10 most visited websites in each category and information about its usage during the month of April 2024. It also contains information on which kind of data was used during the signup.
  - The [html.csv](./dataset/raw_data/html.csv) file acts as an index to reach the HTML files collected at each URL analyzed. Furthermore, it contains the privacy classification of each HTML file. ```private``` refers to whether a page should be private for a certain user, while ```private_details``` refers to whether the HTML file contains private details of a certain user. For example, a homepage that displays the name of the user logged in is public but has private details.
  - The [register_data](./dataset/raw_data/register_data/) folder contains all the details and information used while signing up to each website. For security reasons, passwords were omitted. If you intend to use this dataset for investigation purposes and want to access the accounts, please contact me.
  - The [html_raw](./dataset/raw_data/html_raw/) folder contains all the HTML files as copied from the console dev tools.
  - The [processed](./dataset/processed/) folder contains all the HTML files transformed in order to be used by the LLMs. Namely, [html_no_style_no_script](./dataset/processed/html_no_style_no_script/) stores the transformation where the style and script tags were removed, [html_strings](./dataset/processed/html_strings/) stores the strings extracted from the HTML files and [html_rendered](./dataset/processed/html_rendered/) stores all the images resulting of the renderization of each HTML file.
 
 
- The [models](./models) folder contains all the data used and generated in the scope of running the LLM models themselves. 

[]()
