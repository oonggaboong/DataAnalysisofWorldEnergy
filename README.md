# Data Analysis: World Energy
### <a href="https://github.com/oonggaboong/DataAnalysisofWorldEnergy/blob/main/DataAnalysisofWorldEnergy.ipynb">Python Code in Jupiter Notebook</a>
In this project, I used several Python packages, such as:
- Pandas
- Numpy
- Matplotlib
- Seaborn
- Geopandas
- Folium
- Ipywidgets

<h2>   
    <font color = black >
        <span style='font-family:monospace'>
            Table of Contents
        </span>   
    </font>    
</h2>
<span style='font-family:monospace'>
    <ol>
            <li><a href='#AboutDataset'>About Dataset</a></li>
            <li><a href='#Preparation'>Preparation</a></li>
            <li><a href='#Interpretation'>Data Interpretation</a></li>
            <li><a href='#Scope'>Scope</a></li>
            <li><a href='#Goals'>Goals</a></li>
            <li><a href='#Cleaning'>Data Cleaning and Manipulation</a></li>
            <li><a href='#Modeling'>Modeling and Analysis</a></li>
            <li><a href='#Overview'>World Overview</a></li>
            <li><a href='#Conclusion'>Conclusion</a></li>
</span>
  
<a id="AboutDataset"></a>
<h2>   
    <font color = blue>
        <span style='font-family:monospace'>
            1. About Dataset
        </span>   
    </font>    
</h2>
    
Source: <a href='https://ourworldindata.org/energy'> <b>Our World in Data</b> </a>
(<a href='https://github.com/owid/energy-data'> <b>Github</b> </a>) <br>
Downloaded from the website on 11 October 2023
  
<a id="Preparation"></a>
<h2>   
    <font color = blue>
        <span style='font-family:monospace'>
            2. Preparation
        </span>   
    </font>    
</h2>
Please refer to the <a href="https://github.com/oonggaboong/DataAnalysisofWorldEnergy/blob/main/DataAnalysisofWorldEnergy.ipynb">Jupyter Notebook</a> of the project. <br><br>
    
<a id="Interpretation"></a>
<h2>   
    <font color = blue>
        <span style='font-family:monospace'>
            3. Data Interpretation
        </span>   
    </font>    
</h2>
Please refer to the <a href="https://github.com/oonggaboong/DataAnalysisofWorldEnergy/blob/main/DataAnalysisofWorldEnergy.ipynb">Jupyter Notebook</a> of the project. <br><br>
    
<div class="alert alert-block alert-info">
    <span>
        <b><ins>Insight</ins></b>
        <br>
        <br>
        The dataset consists of 21,861 energy-related entries spanning 305 countries and regions from the year 1900 to 2021, covering 129 distinct fields.
        <br> 
        <br>
        The data types of the columns include object, int64, and float64, and it appears that each field's type aligns appropriately with its content, indicating that no corrections are necessary.
        <br>
        <br>
        However, certain data points are associated with continents, while others pertain to specific regions or segments of continents that can only be accurately interpreted by the dataset's creator. Consequently, not all data can be effectively utilized, requiring a data cleaning process. 
        <br>     
    </span>
</div>
 
<a id="Scope"></a>
<h2>   
    <font color = blue>
       <span style='font-family:monospace'>
            4. Scope
        </span>   
    </font>    
</h2>
The focuses of this analysis are the G7 countries, including the United States, Canada, United Kingdom, France, Germany, Italy, and Japan. The period is from 1990 to 2021.

<a id="Goals"></a>
<h2>   
    <font color = blue>
       <span style='font-family:monospace'>
            5. Goals
        </span>   
    </font>    
</h2>  

The goals of this analysis are: <br>
1. To know which country consumes the most energy.
2. To determine the energy consumption per capita and GDP for each G7 country.
3. To get the portion of energy consumption in the form of electricity.
4. To compare the consumption of primary energy sources (fossil, nuclear, renewable).
5. To analyze the source of energy that has grown the most over the last 30 years.
6. To visualize the energy production patterns in different countries, including the source of energy production, such as coal, gas, oil, or biofuels.
7. To know the relationship among energy production, consumption, and economic indicators, such as GDP, population, and energy consumption per GDP.
8. To discuss the environmental impact of energy production and consumption, including greenhouse gas emissions and carbon intensity of electricity production.
    
    
<a id="Cleaning"></a>
<h2>   
    <font color = blue>
       <span style='font-family:monospace'>
            6. Data Cleaning and Manipulation
        </span>   
    </font>    
</h2>
  
Please refer to the <a href="https://github.com/oonggaboong/DataAnalysisofWorldEnergy/blob/main/DataAnalysisofWorldEnergy.ipynb">Jupyter Notebook</a> of the project. <br><br>
 
    
<p>    
<div class="alert alert-block alert-info">
    <span>
        <b><ins>Insights</ins></b><br><br>
            1. The correlation matrix indicates that electricity is the dominant form of primary energy consumption in G7 nations:<br>
            &nbsp&nbsp&nbsp&nbsp * There is a strong correlation between energy consumption and both electricity demand and generation.<br><br>
            2. It is important to highlight that while electricity represents the largest share of primary energy consumption in G7 countries, these nations do not necessarily focus on domestic generation to satisfy their demand:<br>     
            &nbsp&nbsp&nbsp&nbsp * The share of electricity within total energy consumption <ins>does not</ins> inherently correlate with the level of electricity generation.<br><br>
            3. The G7 countries tend to favor importing electricity rather than producing it from nuclear sources: <br>
             &nbsp&nbsp&nbsp&nbsp * There is a negative correlation between nuclear generation and electricity imports.<br><br>
            4. Additional investigation is necessary to obtain a more comprehensive understanding of these findings, which will be explored in the following sections of the report. <br>
    </span>  
</div>
</p>

<a id="Modeling"></a>
<h2>   
    <font color = blue>
       <span style='font-family:monospace'>
           7. Data Modeling and Analysis
       </span>   
    </font>    
</h2>

<a href="https://github.com/oonggaboong/DataAnalysisofWorldEnergy/blob/main/Plots/P.7.1.jpg"><img align="center" width="auto" height="auto" src="https://github.com/hamid-rahbar/WorldEnergyDataAnalysisPython/blob/main/Plots/P.7.1.4.jpg"></a> <br>

<div class="alert alert-block alert-info">
    <span>
        <b><ins>Insights</ins></b><br><br>
            1. Canada has the highest energy and electricity consumption per capita among the G7 nations, driven by its cold climate, vast geography, and energy-intensive industries, including heavy reliance on electricity for heating and industrial use.<br><br>
            2. G7 countries, particularly France and Japan, are increasing their use of electricity as a cleaner energy source. They have invested heavily in renewable technologies like wind, solar, and hydro, aligning with the global trend toward reducing carbon emissions and meeting climate goals. As a result, the share of electricity in total energy consumption has risen in these nations.<br><br>
            3. Italy is one of the largest electricity importers in the G7, depending on external sources for its energy needs. In contrast, France, Canada, and Germany are significant exporters, with France leading due to its robust nuclear energy infrastructure. Japan, however, maintains energy self-sufficiency, focusing on energy efficiency and investments in nuclear and renewable energy to reduce dependence on imports.<br><br>
    </span>  
</div>



<a href="https://github.com/oonggaboong/DataAnalysisofWorldEnergy/blob/main/Plots/P.7.2.jpg"><img align="center" width="auto" height="auto" src="https://github.com/hamid-rahbar/WorldEnergyDataAnalysisPython/blob/main/Plots/P.7.3.2.png"></a> <br>

<div class="alert alert-block alert-info">
    <span>
        <b><ins>Insights</ins></b><br><br>
            1. U.S. energy consumption has fluctuated over the past decade, reflecting economic conditions, energy prices, and policies. Despite these variations, the share of renewable energy has steadily increased, signaling a shift towards cleaner energy and reduced carbon emissions.<br><br>
            2. Energy consumption in the U.S. declined during the global financial crisis (2008-2009) and the COVID-19 pandemic (2020), highlighting the impact of economic downturns on energy demand. These reductions emphasize the importance of energy efficiency in addressing long-term energy challenges.<br><br>
            3. G7 nations are reducing reliance on nuclear energy and investing in renewables, driven by environmental and health concerns. Japan, after the 2011 Fukushima disaster, significantly decreased its nuclear use, shifting focus to alternative energy sources. Germany and the UK have also seen significant growth in renewable energy adoption, supported by favorable policies and technological advancements.<br><br>
    </span>  
</div>

<a href="https://github.com/oonggaboong/DataAnalysisofWorldEnergy/blob/main/Plots/P.7.3.jpg"><img align="center" width="auto" height="auto" src="https://github.com/hamid-rahbar/WorldEnergyDataAnalysisPython/blob/main/Plots/P.7.4.1.jpg"></a> <br>

<div class="alert alert-block alert-info">
    <span>
        ${\color{blue}Insights:}$<br>
            1. While the United States, the United Kingdom, Germany, Italy, and Japan are still heavily reliant on fossil fuels, both Canada and France have made notable progress in increasing their use of renewable energy. <br>
            2. Despite being primarily based on fossil fuels, Canada and France rank among the highest in renewable energy consumption among the G7 countries. This reflects their efforts to transition towards a cleaner energy mix and reduce their dependence on fossil fuels.  <br>
            3. Additionally, all of the G7 countries have started to reduce their reliance on nuclear energy, reflecting growing concerns about the environmental and health risks associated with nuclear power. These efforts towards reducing the use of fossil fuels and nuclear energy, and increasing investment in renewable energy, demonstrate the commitment of G7 countries to creating a more sustainable and secure energy future.<br>
    </span>  
</div>

<a href="https://github.com/oonggaboong/DataAnalysisofWorldEnergy/blob/main/Plots/P.7.4.jpg"><img align="center" width="auto" height="auto" src="https://github.com/hamid-rahbar/WorldEnergyDataAnalysisPython/blob/main/Plots/P.7.5.1.jpg"></a> <br>

<div class="alert alert-block alert-info">
    <span>
        <b><ins>Insights</ins></b><br><br>
            1. The energy mix for electricity production among the G7 countries varies greatly, with each country having its own unique approach to balancing its energy sources. <br><br>
            2. The United States has long been reliant on fossil fuels for electricity production, but has started to invest in renewable energy sources in recent years. <br><br>
            3. Meanwhile, Canada primarily relies on renewable energy sources for its electricity production.<br><br>
            4. The United Kingdom, Germany, and Italy have been successful in increasing their investment in renewable energy, resulting in a balance between electricity production from fossil and renewable sources.<br><br> 
            5. France primarily relies on nuclear power for electricity production.<br><br>
            6. Japan continues to rely heavily on fossil fuels, with an increase in the use of fossil fuels for electricity production following a reduction in the use of nuclear energy. <br><br>
            7. These differences reflect the diverse energy needs, resources, and priorities of the G7 countries, and highlight the importance of developing a flexible and diverse energy mix that can meet the needs of different countries and regions.<br><br>
    </span>  
</div>

<a href="https://github.com/oonggaboong/DataAnalysisofWorldEnergy/blob/main/Plots/P.7.5.jpg"><img align="center" width="auto" height="auto" src="https://github.com/hamid-rahbar/WorldEnergyDataAnalysisPython/blob/main/Plots/P.7.6.1.jpg"></a> <br>

<div class="alert alert-block alert-info">
    <span>
        <b><ins>Insights</ins></b><br><br>
            1. Each G7 nation exhibits unique strengths and focal points regarding renewable energy sources.<br><br>
            2. The United States predominantly utilizes hydropower within its renewable energy portfolio, while solar energy has seen substantial growth in recent years.<br><br>
            3. Canada’s renewable energy framework is largely centered on hydropower, complemented by a smaller share of wind energy.<br><br>
            4. In contrast, the United Kingdom and Germany primarily depend on wind energy, whereas France relies mainly on hydropower but has also witnessed a rise in wind energy utilization.<br><br>
            5. Italy's energy strategy is chiefly anchored in hydropower, although there has been a notable increase in solar energy adoption.<br><br>
            6. Japan's renewable energy landscape is significantly supported by hydropower, alongside a marked rise in solar energy in recent years.<br><br>
            7. These variations underscore the distinct energy requirements, available resources, and strategic priorities of each G7 country, emphasizing the necessity for a versatile and varied energy mix capable of addressing the diverse needs of different nations and regions.<br><br>
    </span>  
</div>

<a id="Overview"></a>
<h2>   
    <font color = blue>
        <span style='font-family:monospace'>
            8. World Overview
        </span>   
    </font>    
</h2>

<a href="https://github.com/oonggaboong/DataAnalysisofWorldEnergy/blob/main/Plots/P.8.1.jpg"><img align="center" width="auto" height="auto" src="https://github.com/hamid-rahbar/WorldEnergyDataAnalysisPython/blob/main/Plots/P.8.1.jpg"></a> <br>

<a id="Conclusion"></a>
<h2>   
    <font color = blue>
        <span style='font-family:monospace'>
            9. Conclusion
        </span>   
    </font>    
</h2>

<div class="alert alert-block alert-info">
    <span>
        <b><ins></ins></b><br>
        Among the G7 countries, the United States is the country that consumes the most energy. However, as of the most recent data, China has the highest energy consumption, followed by the United States. This is primarily due to China's large population, rapid industrialization, and increasing demand for energy. Other large consumers include India and Russia.<br><br>

In terms of energy consumption per capita, Canada ranks first among the G7. However, globally, smaller countries like Qatar, Kuwait, and the United Arab Emirates are leading due to their high energy use compared to their small population sizes.<br><br>

There are a lot of things that we can discuss regarding energy in this world. With the right data analysis technique, we can get the answers to our questions and tackle the problems that appear. 
    </span>  
</div>
