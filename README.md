# Manning_liveProject
## Discovering Disease Outbreaks from News Headlines


Identifying and mapping epidemics is crucial to prevent or respond to deadly disease outbreaks. Your first assignment for the WHO is as follows:

- Extract the locations (city and/or country name) from each news headline.
- Find the geographic coordinates of each headline using the city/country.
- Cluster (group) the headlines based on the geographic location.
- Visualize the clusters on a map and analyze them for patterns indicating an epidemic.
- Investigate the largest clusters for signs of disease outbreaks.
- Review headlines in the largest clusters within the United States and around the world. If any disease outbreak is   particularly dominant, visualize all worldwide mentions of that disease.
- Provide a summary of your findings to your superiors at the WHO so they can direct resources.


The project is broken into five parts.

1. Extracting City and Country Information from News Headlines

2. Finding Geographic Locations of Headlines

3. Clustering Headlines Based on Location

4. Identifying Disease Outbreaks

5. Presenting the Disease Outbreak Data

The skills covered in order are the following: 
- text extraction
- data manipulation
- clustering
- interpreting algorithm outputs
- producing an actionable report. 

The deliverable from each part is a Jupyter notebook (uploaded to GitHub) documenting your workflow and results. 
The final executive summary will be a notebook converted to html or a PDF to share the conclusions with your superiors at the WHO. 
Each section builds upon the previous and will test your skills in a different area of data science. 

As you go through the project, keep in mind the **overall objective: to identify disease outbreaks around the world.** The project is representative of the problems solved by data scientists in industry or academia and utilizes the most popular tools for data science in Python.

**Dataset**

**[headlines.txt](https://livevideo-resources.s3-us-west-2.amazonaws.com/course-data/93/headlines.txt)** (Available in the GitHub repository)

This file contains a curated list of actual worldwide news headlines referring to diseases.

Each headline is on a separate line with a total of 650 headlines.
> Example headlines:
>
> - Zika spreads to Winter Park
> - Durango is infested with Hepatitis B
> - Mpika authorities confirmed the spread of Chikungunya
> - Gladstone Encounters Severe Symptoms of Dengue
> - Mad Cow Disease Hits London
> - Zika symptoms spotted in Quito 

The headlines in the dataset were synthetically created, but the dataset’s distribution of disease and location-mentions is modeled on real health mentions in news articles over the first few months of 2016. These articles were detected by matching health keywords within international sections of popular online news sources. Such sections are commonly demarcated by continent or country within the news source’s URL. For instance, https://cnn.com/africa contains English-language news coverage from Africa, while https://reuters.com/places/thailand contains English-language news coverage from Thailand. Article content ranges from local politics to newsworthy health incidents.

We matched health terms in the body and headline of the articles to find the health-related articles. Inclusion of the body text would have added surplus noise to our analysis and all mentions of location-specific diseases have been transformed into simple, single-line article titles. About half of the headlines originated in the United States, which might necessitate splitting the data into two categories: The United States and the rest of the world.

