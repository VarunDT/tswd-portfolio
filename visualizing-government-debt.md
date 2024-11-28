| [Home Page](https://varundt.github.io/tswd-portfolio/) | [Visualizing Debt](https://varundt.github.io/tswd-portfolio/visualizing-government-debt) | [Critique by Design](https://varundt.github.io/tswd-portfolio/critique-by-design) | [Final Project I](https://varundt.github.io/tswd-portfolio/final-project-part-one) | [Final Project II](https://varundt.github.io/tswd-portfolio/final-project-part-two) | [Final Project III](final-project-part-three) |

# Visualising Government Debt

This assignment covers three different ways to visualize the same data and steps on how to recreate the data visualization. In the end, there is also an explanation on why a particular visualisation works best in explaining the particular part of the data.

## Part One: Working with web-based visualization tools and data

To replicate this visualization, follow these steps:
1. Visit the [OECD data site](https://www.oecd.org/en/data.html). You’ll see a few featured visualizations on the main page.
2. In the search bar, type "government debt" and select "General government debt" from the results to access the government debt-to-GDP ratio data.
3. Review the summary description and explore the chart. Hover over a bar to see specific data, and click on countries to highlight them in different colors.
4. Adjust the slider below the graph to display data for a single year. Move the slider to find a recent year with comprehensive data (e.g., I have selected 2019 for this embedded image).
5. To download the chart, click the three-dot icon in the top right corner, and choose the .png option to save the image to your device.


![General Government Debt as % of GDP (2019)](https://github.com/VarunDT/tswd-portfolio/blob/c48f5afa91fb93b3861f85284621964d34bfe0f2/OECD%3AGGD?raw=true)

## Part Two: Working with Tableau

To replicate this process in Tableau:
1. **Download Data**: Save the OECD dataset from the previous link.
2. **Open Data in Tableau**: Launch Tableau Desktop. Under "Connect," select "Text file" and open your saved OECD dataset.
3. **Set Date Format**: If the "Time" column is read as a number, click the "#" icon above it and select "Date", to save it as a Year.
4. **Create Data Extract**: Under "Connection," select "Extract" to enable publishing later.
5. **Go to Worksheet**: Click "Go to Worksheet" above the "Sheet 1" tab.
6. **Build a Line Chart**:
   - Drag "Time" to Columns and "Value" to Rows.
   - Drag "Location" to the Marks card.
7. **Switch to Highlight Table**:
   - In "Show Me," select "Highlight Tables."
   - Tableau will auto-add fields for a heatmap view of debt-to-GDP ratios.
8. **Sort Data**: Click the "Location" dropdown, choose "Sort," then sort by "Field" in "Descending" order, with "Average" aggregation.
9. **Customize Colors**:
   - In the Marks card, click "Color" > "Edit Colors."
   - Select "Orange-Blue Diverging," check "Reversed," and set 100 as the center value.
10. **Filter Out Missing Data**: Remove Colombia by clicking "Location" > "Filter" and unselecting "COL", since it has no data
11. **Finishing Touches**: Rename the sheet, add a data source citation, and save the workbook.

<div class='tableauPlaceholder' id='viz1730766615644' style='position: relative'>
    <noscript>
        <a href='#'>
            <img alt='GENERAL GOVERNMENT DEBT FOR DIFFERENT LOCATIONS OVER TIME (1995-2019) SOURCE: OECD GENERAL GOVERNMENT DEBT (https://www.oecd.org/en/data/indicators/general-government-debt) DEFINITION: General government debt is the gross debt of the general government as a percentage of GDP.' src='https://public.tableau.com/static/images/OE/OECDGOVTDEBT/Sheet1/1_rss.png' style='border: none' />
        </a>
    </noscript>
    <object class='tableauViz' style='display: none;'>
        <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
        <param name='embed_code_version' value='3' />
        <param name='site_root' value='' />
        <param name='name' value='OECDGOVTDEBT/Sheet1' />
        <param name='tabs' value='no' />
        <param name='toolbar' value='yes' />
        <param name='static_image' value='https://public.tableau.com/static/images/OE/OECDGOVTDEBT/Sheet1/1.png' />
        <param name='animate_transition' value='yes' />
        <param name='display_static_image' value='yes' />
        <param name='display_spinner' value='yes' />
        <param name='display_overlay' value='yes' />
        <param name='display_count' value='yes' />
        <param name='language' value='en-GB' />
        <param name='filter' value='publish=yes' />
    </object>
</div>
<script type='text/javascript'>
    var divElement = document.getElementById('viz1730766615644');
    var vizElement = divElement.getElementsByTagName('object')[0];
    vizElement.style.width = '100%';
    vizElement.style.height = (divElement.offsetWidth * 0.75) + 'px';
    var scriptElement = document.createElement('script');
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
    vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>


## Part Three: create your own visualization

To create a box and whisker plot in Tableau based on your previous sheet:
1. **Duplicate Sheet**: Right-click on "Sheet 1" in the sheet tabs at the bottom and select "Duplicate" to create a copy of the original sheet.
2. **Select Box and Whisker Plot**: In the "Show Me" panel on the right, choose "Box and Whisker Plot."
3. **Relabel the Axes**: Double-click on each axis title to rename them appropriately (e.g., "Year" for the x-axis and "Debt-to-GDP Ratio" for the y-axis).
4. **Customize Box Appearance**:
   - Click on the box plot, and then click on "Edit"  toselect the style, color and adjust the opacity slider to set the transparency level for the box.
   - Customize the borders and box thickness as needed.
5. **Format Location Points**:
   - Click on the individual data points (location points) within the Marks card.
   - Adjust the color, opacity, and size to make them visually distinct and ensure they stand out from the boxes.
6. **Adjust Axis Width and Ticks**:
   - Right-click on each axis, select "Edit Axis," and modify the range, tick marks, and width to your preference for clearer data presentation.

This will create a customized box and whisker plot that allows for easy visual comparison of the max, min and average Debt-to-GDP ratios over time.

<div class='tableauPlaceholder' id='viz1730766365733' style='position: relative'>
    <noscript>
        <a href='#'>
            <img alt='DISTRIBUTION OF GENERAL GOVERNMENT DEBT OVER TIME (1995-2019) SOURCE: OECD GENERAL GOVERNMENT DEBT (https://www.oecd.org/en/data/indicators/general-government-debt) DEFINITION: General government debt is the gross debt of the general government as a percentage of GDP.' src='https://public.tableau.com/static/images/OE/OECDGOVTDEBTPLOT2/Sheet12/1_rss.png' style='border: none' />
        </a>
    </noscript>
    <object class='tableauViz' style='display: none;'>
        <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
        <param name='embed_code_version' value='3' />
        <param name='site_root' value='' />
        <param name='name' value='OECDGOVTDEBTPLOT2/Sheet12' />
        <param name='tabs' value='no' />
        <param name='toolbar' value='yes' />
        <param name='static_image' value='https://public.tableau.com/static/images/OE/OECDGOVTDEBTPLOT2/Sheet12/1.png' />
        <param name='animate_transition' value='yes' />
        <param name='display_static_image' value='yes' />
        <param name='display_spinner' value='yes' />
        <param name='display_overlay' value='yes' />
        <param name='display_count' value='yes' />
        <param name='language' value='en-GB' />
        <param name='filter' value='publish=yes' />
    </object>
</div>
<script type='text/javascript'>
    var divElement = document.getElementById('viz1730766365733');
    var vizElement = divElement.getElementsByTagName('object')[0];
    vizElement.style.width = '100%';
    vizElement.style.height = (divElement.offsetWidth * 0.75) + 'px';
    var scriptElement = document.createElement('script');
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
    vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

## Explaining the Visualizations

This section summarizes different visualization methods used to analyze the OECD's "General Government Debt" data. We created three visualizations—a bar chart(sourced from the website), a heatmap (professor’s choice), and a box plot (personal choice). Each plot offers insights into how countries' debt-to-GDP ratios have evolved from 1995 to recent years.

The bar chart on the OECD website includes a complementary slider to adjust the year, allowing a focused view of each year and a magnified view of each country's data for that particular year. While this is useful for examining individual years, but combining all bar charts over time would make it difficult to extract meaningful trends. The heatmap effectively highlights high and low debt levels across countries and years, with color shades making it easy to spot trends. We can set any averag value we want and see how the data revolves around that average value. This approach allows for quick, comparative analysis not only for data of a particular location for different years, but also across multiple locations at the glance-of-an-eye. This approach is better than the first one as it occupies lesser space and the viewer's task is limited, but it lacks details on overall data spread and outliers. The box plot addresses this limitation by showing the distribution of the data for each year, including median values, ranges, and outliers. It provides a clearer picture of typical range of debt values while revealing variations for the given countries over time. This chart also helps identify highlight any extreme cases or high variance between countries. I personally chose the box plot, because the first 2 plots were very focused on particular locations, but the box plot gives a more overall idea of how the debt fluctuates over the years and also how much the average debt of all countries shifts as the years progress.






