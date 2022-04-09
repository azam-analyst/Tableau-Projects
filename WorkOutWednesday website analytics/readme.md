# Website analytics of Work our Wednesday on Tableau

This is a data analysis project based on the google analytics data of Work Out Wednesday which is a weeklay challenge site to re-create data visualization posted by other competitors. the dataset contains records of website traffic informaton on different dates from 2019 to 2021.

**Dataset:** The dataset for the project is collected from data.world website.Linke:https://data.world/annjackson/wow-google-analytics?msclkid=e883caaeb85711ecb70515d920d34da3.  The dataset contains 10 column with 33,865 rows of records. 
Columns are: Country,date,source/medium,bounces,exits,pageviews,session duration,sessions,time on page,unique pageviews.

To draw out findings and insights from the project some major google analytics KPIs have been analysed are-
1.Average bounce rate, 
2.Average session duration
3.Average pageviews
4.Average time on page

**KPI calculation process in Tableau:**

1.Average bounce rate: A new calculated field were created named bounce rate% where the formula used was (SUM([Bounces])/SUM([Sessions])) which gives the bounce rate per session. The fractional value was converted to percentage from format menu in tableau for the bounce rate% field.

2.Average session duration: The avarge value of session duration field AVG(session Duration).

3.Average pageviews per session: By creating calculated field and puting the formula SUM([Pageviews])/SUM([Sessions]) gives the Avergae pageviews per session which means how many pages on avergae were viewd on session.

4.Average time on page: The avarage value of time on page field  AVG(Time on page)

![Work Out wednesday 1](https://user-images.githubusercontent.com/96620728/162594327-970b9b58-f1fc-469c-8713-2afedcf961f9.png)

**Findings from the data analysis:**

**Number of session by countries:** From the filled map in tableau it was found that the highest number of sessions and pageviews came from **United states** with very impressive 57,499 sessions through 2019 to 2021. The second postion is hold by India with **25,360** sessions. Undoubtedly these two countries has really high popularity for work out wednesday competition.

**Total Pageviews | Average page views per session:** The idea of creating this barchart was to find total pagevies and avergae page views per session done by visitors coming from difference source and mediam. The highest number of visitors accesed the website from organically searching by google and the average page viws was really good at **2.9** pages per session. Google was followed by bing and yahoo in organic search category. 

**Total Pageviews | Average page views per session**:In refferal category the most pageviews were made from visitors coming from twitter but visitors from pinterest.com alothough had a good number pageviews but the pageviews per session were very low at **1.2.** 

The avergae time spent per page by visitors from pinterest was also low with only 24 seconds per page with a very high bounce rate of 84%.

**Sessions|Bounce rate for different Mediums**:Overall, the visitors coming from **organic searches** had a good bounce rate of **37.69%** meaning they tend to be exploring more pages and not just goinf of after visiting first page. Visitors coming from direct search had little bit high bounce rate of **51%** followed by visitors by referral sites at 47.63%

**Number of Sessions over the years**: While analysing number of sessions over the years by line graph it was very interestingly visible that the website session tends to be at high in **January** over the years and tend to be going down afterwards the again rising at the end of the year. 

**Major insights from the analysis:**

The visitors coming from pinterest.com mostly were not very much reactive with the website with very high bounce rate, average session duration per page and average pageviews per sesssion.

Visitors coming through organic search by quant.com tend to be spending more time on each page at 1114 seconds/page although the number of sessions were 106.
The activity on the website tend to go high at the beginning of the year then gradually decreasing on the mid year,again rising up at the end of the year.

Overall, Work Out Wednesday site had an above average bounce rate of **44.31%** with a very good pageviews per session at **2.6 **

The tableau dashboard can be viewd here: https://public.tableau.com/views/WOW_16485832068510/Dashboard1
