# Assignment 4

### Original Data Viz
This visualization is available in the [European Medicines Agency 2010 Report](https://www.ema.europa.eu/en/documents/report/sales-veterinary-antimicrobial-agents-19-european-union/european-economic-area-countries-2010-second-european-surveillance-veterinary-antimicrobial_en.pdf) on antimicrobial agents used for animals in Europe. I chose this visualization because the stacked bar chart type is not suitable in this context where there are 11 categories for each country. There is a lot of eye travel and the message is not instantly clear.

![Assignment4image](https://user-images.githubusercontent.com/116593921/202044462-70bf5724-940b-4f59-a7c0-35c801b21c0d.PNG)


### Summary of Sketch
I redesigned the visualization on Figma and made the following modifications:
1) Changed the title to a shorter version which is easier to read and understand.
2) Changed bar segments to circles which are more visible.
3) Used a brighter color palette so circles are easily distinguishable.
4) Added a note for the y-axis explaining PCU for non-technical audience.

![Assignment4sketch](https://user-images.githubusercontent.com/116593921/202045697-ef2b0de4-c7ae-4543-a64f-84dfeec1ef9d.PNG)

### User Feedback
I interviewed two people to get feedback on my sketch. 


#### _Interviewee-1 (Female; Non-technical background; Age early 30s)_

**Can you tell me what you think this is?**

I think the graph shows the quantity of antimicrobial agents sold in different European countries in 2010

**Can you describe to me what this is telling you?**

It's showing how many mgs or PCUs of each category of an antimicrobial unit was sold in different European countries in 2010

**Is there anything you find surprising or confusing?**

The size of the circles is very confusing. Not sure why the circles are getting larger as the mgs/pui increases. The colors are also confusing because there is not a lot of difference between them. This might've been better shown as a graph?

**Who do you think is the intended audience for this?**

Perhaps the sellers or marketers of antimicrobial agents in Europe.

**Is there anything you would change or do differently?**

Maybe use a line graph 📉  instead of the circles with clear demarcation of different categories


#### _Interviewee-2 (Male; Technical background Age late 20s)**_

**Can you tell me what you think this is?**


**Can you describe to me what this is telling you?**


**Is there anything you find surprising or confusing?**


**Who do you think is the intended audience for this?**


**Is there anything you would change or do differently?**



### Feedback from in-class exercise

_**What Didn't Work:**_ The sketch still has too many categories which make it hard to understand. There is still a lot of eye travel because of the colors.

_**What Questions Came Up:**_ Is it really important for the reader to know the exact antimicrobial category names? If not, then we don't have to have a diverging color palette; try highlighting a few antimicrobial classes that are the most harmful.

_**What New Inspiration Arose:**_ If it is a stacked bubble chart then order the countries (highest to lowest) that use the antimicrobial agents. Try grouping together the 11 antimicrobial categories into 2 or 3 that are commonly known. The reader might not be too interested in knowing the category names.


## Redesign
Feedback from interviewees suggests that the title and message is clear, however, the redesign using a bubble chart is still creating confusion and takes time to interpret what the visualization means. Based on the feedback from two interviewees and in-class exercise, I have made two versions of the redesign.


### First Redesign
In this first redesign similar to my sketch, I have reduced the use of colors by highlighting only those antimicrobial categories that are known to be most harmful. This information was taken from two external sources ([Source 1](https://www.frontiersin.org/articles/10.3389/fmicb.2016.01626/full), [Source 2](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7139321/)). Two modifications were not possible for this visualization in Tableau; 1) I was not able to order the countries on x-axis because the series on y-axis are more than one and 2) I was not able to add a note to the visualization as a Footer because that option is only available in the Dashboard option. I could add a caption to the chart but then I was not able to delete the title 'Caption' which did not look nice.

<div class='tableauPlaceholder' id='viz1668554901992' style='position: relative'><noscript><a href='#'><img alt='Sales of antimicrobial classes for animals in Europe in 2010. ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;As&#47;Assignment_4_16685533290910&#47;Sheet1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Assignment_4_16685533290910&#47;Sheet1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;As&#47;Assignment_4_16685533290910&#47;Sheet1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object></div><script type='text/javascript'>var divElement = document.getElementById('viz1668554901992');var vizElement = divElement.getElementsByTagName('object')[0];vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';var scriptElement = document.createElement('script');scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';vizElement.parentNode.insertBefore(scriptElement, vizElement);</script>



### Second Redesign
In the second redesign, I have used a map in Flourish to plot the antimicrobial agents one at a time. The original visualization looks busy because 11 categories are presented for each of the 18 countries. To make it simple and intuitive, I decided to show one antimicrobial class at a time and add a drop-down option to select the category of antimicrobial class. The color palette is red because it signifies a worrying situation. The legend goes from light red to dark red following general convention for numbers/percentages.

<div class="flourish-embed flourish-map" data-src="visualisation/11833156"><script src="https://public.flourish.studio/resources/embed.js"></script></div>


