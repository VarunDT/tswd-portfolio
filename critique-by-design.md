| [Home Page](https://varundt.github.io/tswd-portfolio/) | [Visualizing Debt](https://varundt.github.io/tswd-portfolio/visualizing-government-debt) | [Critique by Design](https://varundt.github.io/tswd-portfolio/critique-by-design) | [Final Project I](final-project-part-one) | [Final Project II](final-project-part-two) | [Final Project III](final-project-part-three) |

# Redesigning Data Visualizations: A Critique-by-Design Approach
In this project, I followed a structured critique-by-design process to enhance a data visualization through five key steps:

**1. Selecting a Visualization for Redesign:** I chose a visualization from MakeoverMonday that presented opportunities for improvement in clarity and readability.

**2. Critiquing the Original Visualization:** I evaluated the visualization’s strengths and weaknesses, noting issues such as readability, color scheme, clutter, and interpretability. This critique helped me identify specific areas to improve.

**3. Sketching a New Design:** Using the data provided on the visualization’s website and my critique, I created a basic sketch and experimented with different layouts to make the information clearer and more accessible.

**4. Gathering User Feedback:** I shared my sketch with others to assess its clarity compared to the original. Their feedback provided valuable insights, allowing me to refine my design further.

**5. Building the Final Version:** Using Tableau, I developed the final visualization, incorporating feedback to ensure a simple, clear, and effective data story.


## Step one: The Visualization
From the MakeoverMonday website, I selected the following article:

**Source:** [Visual Capitalist - Ranked: The Most Reliable Car Brands in the U.S.](https://www.visualcapitalist.com/ranked-the-most-reliable-car-brands-in-the-u-s/)  
**Published by:** Marcus Lu on Visual Capitalist, July 18, 2024  
**Graphic by:** Sam Parker  

**Original Visualization:**
![Most-Dependable-Car-Brands-in-the-US_Web](https://github.com/user-attachments/assets/bda06976-1dc8-40a1-9586-ee1e55353bf7)

I selected this data visualization because it presents valuable information on vehicle reliability, a crucial consideration for consumers in the U.S. automotive market. The visualization displays a ranking of car brands based on the number of reported issues per 100 vehicles, derived from J.D. Power’s 2024 U.S. Vehicle Dependability Study. The study collected data from over 30,000 owners of 2021 model-year vehicles, analyzing various problem categories such as exterior, interior, infotainment, and driving experience.

This visualization has potential but could be improved in terms of readability, layout, and data interpretation. I believe that with a few adjustments, the information could be presented more effectively, making it easier for viewers to understand at a glance. This selection aligns with my goal of enhancing clarity and storytelling in data visualizations, particularly by addressing common user experience challenges.

## Step two: The Critique
This critique applies Stephen Few's "Data Visualization Effectiveness Profile" to analyze and evaluate the visualization. The primary audience includes car buyers, car owners, and automotive industry professionals interested in vehicle reliability, valuing clear, comparable information to make informed choices. The visualization is somewhat effective in delivering quick, at-a-glance insights into the reliability of different car brands, helping viewers gauge brand performance based on "problems per 100 vehicles." Elements that work well include the dark background and bold, white text, which create visual appeal, and the use of brand logos, which makes the visualization relatable and engaging. Numeric values beside each brand support quick understanding of each brand's ranking, while the bar chart format is well-suited for comparison. However, there are areas for improvement: the two-column layout complicates readability by requiring viewers to scan across both columns to grasp the full ranking, which could be simplified by restructuring into a single-column layout. Additionally, the color gradient, though visually engaging, does not correlate directly with reliability scores, and a more intuitive color scheme (such as green for higher reliability and red for lower) could make the data easier to interpret. Adding an industry average benchmark would offer a reference point for better comparison. Overall, this critique-by-design method effectively highlighted the visualization’s strengths and areas for improvement, making it clear that adjustments to layout, color, and comparison features would enhance clarity, usefulness, and engagement for the audience.

## Step three: Sketch a Solution
<img width="1317" alt="Screenshot 2024-11-10 at 6 08 46 PM" src="https://github.com/user-attachments/assets/cd72229e-0ba6-4bf4-ab6c-1ce34a8a5c4a">
This is a basic visualization of the data provided on the original website. To create it, I simply uploaded the data to Tableau, selected the chart type, edited the axes, and chose a color scheme to match the story I wanted to present.

## Step four: Test the Solution

To evaluate the effectiveness of my redesigned visualization, I shared it with several colleagues, my roommates and my parents (10 viewers in total) and gathered their feedback on its clarity and usability. I used open-ended questions to determine whether the visualization communicated the data clearly without requiring additional explanation. Below are the questions I asked, followed by the key feedback and insights gathered.

**Questions Asked During the Feedback Session**

1. Can you tell me what you think of this visualization compared to the original one?
2. Can you describe what story this visualization is trying to tell you?
3. Is there anything you find surprising or confusing in this chart?
4. If given the chance, is there anything you would change or do differently?
5. Do the colors, layout, and text provide enough clarity for you to understand the rankings?

**Key Feedback Received and Insights**

**1. Misleading Title**: The title, “Most Reliable Car Brands,” could be misleading, as it doesn’t make it immediately clear that fewer problems indicate higher reliability. Although the subtitle mentions that fewer problems mean more reliability, this could be overlooked. A more explicit title, such as “Car Brands Ranked by Fewest Problems per 100 Vehicles,” would help eliminate ambiguity. An additional line reinforcing that “higher on the list indicates fewer problems and thus higher reliability” would assist first-time viewers in correctly interpreting the data.

**2. Color Usage**: The color scheme, which transitions from green (fewer problems) to red (more problems), was well-received for intuitively communicating reliability, with green symbolizing better performance and red indicating worse.

**3. Ranking Ambiguity**: There was some initial uncertainty about the ranking direction due to the top-down order of the bars, which might be interpreted in different ways. Adding small markers or text labels, like “Most Reliable” at the top and “Least Reliable” at the bottom, would clarify the ranking, making it immediately clear that brands at the top are more reliable than those at the bottom, especially for viewers unfamiliar with the data source.

**4. Average Line/Bar and it's Visibility**: Although the average bar is distinct, it doesn’t stand out as much as expected and may blend into the design. Using a different type of line to highlight it or make it more prominent, along with extending the line horizontally across all bars, would enhance its visibility as a benchmark, allowing viewers to more easily compare each brand’s reliability against the industry average.

**5. Visual Overload or High data density**: The number of brands included in the chart made it appear visually overwhelming. A recommended approach was to categorize brands into segments, such as “Top 5 Most Reliable” and “Bottom 5 Least Reliable,” and display only those. This would reduce the amount of data presented at once, highlighting the brands that are extreme outliers in terms of reliability, making it easier for viewers to interpret the information without getting lost in details.

**6. Flag Usage and Font Size**: The inclusion of country flags next to each brand was seen as unnecessary, as the country of origin isn’t directly relevant to reliability. Removing the flags would reduce visual clutter and streamline the design. Additionally, increasing the font size for brand names would improve readability, especially for viewers on smaller screens.

**7. Metric Presentation**: The x-axis metric, “Problems per 100 Vehicles,” focuses on issues rather than direct reliability, which could be confusing for some viewers. Inverting the metric or using a “Reliability Score,” where higher scores represent better reliability, was suggested. However, due to the lack of direct data for a reliability score, this change may require additional data or recalculations. If inverting isn’t possible, adding a small note explaining the metric’s significance and how it relates to reliability would help viewers interpret the data more effectively. 


## Step five: Build the Solution

<div class="tableauPlaceholder" id="viz1731553478181" style="position: relative">
    <noscript>
        <a href="#">
            <img 
                alt="CAR BRANDS RANKED BY PROBLEMS PER 100 VEHICLES (Source: J.D. Power 2024) NOTE: CARS WITH FEWER PROBLEMS THAN THE AVERAGE ARE CONSIDERED MORE RELIABLE" 
                src="https://public.tableau.com/static/images/CA/CARASSIGNMENT-PLOT1/Sheet1/1_rss.png" 
                style="border: none" 
            />
        </a>
    </noscript>
    <object class="tableauViz" style="display: none;">
        <param name="host_url" value="https%3A%2F%2Fpublic.tableau.com%2F" />
        <param name="embed_code_version" value="3" />
        <param name="site_root" value="" />
        <param name="name" value="CARASSIGNMENT-PLOT1/Sheet1" />
        <param name="tabs" value="no" />
        <param name="toolbar" value="yes" />
        <param name="static_image" value="https://public.tableau.com/static/images/CA/CARASSIGNMENT-PLOT1/Sheet1/1.png" />
        <param name="animate_transition" value="yes" />
        <param name="display_static_image" value="yes" />
        <param name="display_spinner" value="yes" />
        <param name="display_overlay" value="yes" />
        <param name="display_count" value="yes" />
        <param name="language" value="en-GB" />
        <param name="filter" value="publish=yes" />
    </object>
</div>
<script type="text/javascript">
    var divElement = document.getElementById("viz1731553478181");
    var vizElement = divElement.getElementsByTagName("object")[0];
    vizElement.style.width = "100%";
    vizElement.style.height = (divElement.offsetWidth * 0.75) + "px";
    var scriptElement = document.createElement("script");
    scriptElement.src = "https://public.tableau.com/javascripts/api/viz_v1.js";
    vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>
<br>

<div class="tableauPlaceholder" id="viz1731552678369" style="position: relative">
    <noscript>
        <a href="#">
            <img 
                alt="FIVE BEST AND WORST CAR BRANDS IN THE US BASED ON RELIABILITY (Source: J.D. Power 2024) NOTE: THE 0 ON THE X-AXIS REPRESENTS THE AVERAGE NUMBER OF PROBLEMS PER 100 VEHICLES THAT A CAR BRAND TYPICALLY EXPERIENCES. CARS BRANDS WITH FEWER PROBLEMS THAN THIS AVERAGE ARE CONSIDERED MORE RELIABLE" 
                src="https://public.tableau.com/static/images/CA/CARASSIGNMENT-PLOT2/Sheet2/1_rss.png" 
                style="border: none" 
            />
        </a>
    </noscript>
    <object class="tableauViz" style="display: none;">
        <param name="host_url" value="https%3A%2F%2Fpublic.tableau.com%2F" />
        <param name="embed_code_version" value="3" />
        <param name="site_root" value="" />
        <param name="name" value="CARASSIGNMENT-PLOT2/Sheet2" />
        <param name="tabs" value="no" />
        <param name="toolbar" value="yes" />
        <param name="static_image" value="https://public.tableau.com/static/images/CA/CARASSIGNMENT-PLOT2/Sheet2/1.png" />
        <param name="animate_transition" value="yes" />
        <param name="display_static_image" value="yes" />
        <param name="display_spinner" value="yes" />
        <param name="display_overlay" value="yes" />
        <param name="display_count" value="yes" />
        <param name="language" value="en-GB" />
        <param name="filter" value="publish=yes" />
    </object>
</div>
<script type="text/javascript">
    var divElement = document.getElementById("viz1731552678369");
    var vizElement = divElement.getElementsByTagName("object")[0];
    vizElement.style.width = "100%";
    vizElement.style.height = (divElement.offsetWidth * 0.75) + "px";
    var scriptElement = document.createElement("script");
    scriptElement.src = "https://public.tableau.com/javascripts/api/viz_v1.js";
    vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>
<br>

**Final Step Summary**

In response to the feedback, I implemented several adjustments in the final redesign to enhance clarity, accessibility, and overall user experience. First, the title was revised to more explicitly convey that the visualization ranks car brands by “problems per 100 vehicles,” providing immediate context and eliminating any potential ambiguity around the data’s focus. This change was essential to ensure that viewers understood that the chart highlights brands with fewer reported issues as the most reliable. The color scheme was another major area of improvement. Additionally, I added labels on the right side of the chart indicating “More Reliable” at the top and “Less Reliable” at the bottom. These labels provide immediate context for viewers, helping them to interpret the color scheme and ranking direction without needing further explanation. Emphasizing the industry average was another critical improvement. I used a dashed line to represent the average, extending it  across the chart to provide a clear benchmark. This line makes it easier for viewers to assess each brand’s reliability relative to the industry standard, allowing them to see at a glance which brands perform above or below average. To streamline the visualization and reduce distractions, I removed unnecessary elements, such as country flags next to brand names. Since the country of origin wasn’t directly relevant to reliability, omitting these flags reduced visual clutter and allowed viewers to focus on the data itself. Furthermore, I increased the font size for brand names to enhance readability, ensuring that the chart remains accessible and easy to read across various devices and screen sizes. I would have also loved to integrate the logos into the visualization, but it felt really tedious to do that in Tableau. ANother unresolved issue was the bar width, but I feel like the second visualization solves that.

The purpose of the first visualization is to give users a comprehensive comparative analysis of various car brands in the market, focusing on their reliability relative to one another. This approach allows viewers to quickly see how brands perform against each other based on the number of reported problems per 100 vehicles. It serves as a practical tool for consumers who are considering different car brands, helping them identify which brands stand out as more reliable. 

For the second visualization, I focused on creating a simplified view that highlights only the five most reliable and five least reliable brands. Using a horizontal bar chart, this visualization shows each brand’s deviation from the industry average, allowing viewers to quickly identify the best and worst performers. Brands that perform better than average are represented with bars extending to the left (in blue), while those that perform worse extend to the right (in gray). This simplified view caters to viewers who may prefer a quick summary of the best and worst performers without needing to analyze the entire dataset. 

<br>
***AI USAGE NOTE:*** I used ChatGPT and Grammarly to assist with grammar and enhance the professionalism of the text.




