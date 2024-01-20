# Exploratory Data Analysis (EDA)

<p align="justify"><b>Exploratory Data Analysis (EDA) </b>is the process of summarizing data using statistical and graphical approaches in order to highlight relevant features of that data for further examination. This entails analyzing the dataset from several perspectives and characterizing and summarizing it without making any assumptions about its contents.
Before entering into statistical modeling or machine learning, exploratory data analysis is a critical step to check the data is what it claims to be and that there are no evident flaws. Every organization's data science efforts should include it.</p>

Description: <b>Exploratory Data Analysis for California, Iran and Indonesia Earthquake</b>

<p align="justify"><b>Using EDA</b>, we can readily interpret the dataset, uncover patterns, identify outliers, and investigate the relationship between variables using non-graphical and graphical methodologies. EDA is a critical component of a data science project for understanding data and gaining insight into each variable.</p>

<b>Table of Contents</b>
1. Feature Description
2. Correlation Variable
3. Data Visualization
4. Break down Earthquake map into grid (1 x 1) degree
5. Count Number earthquake each grid
6. Statistical Description of Earthquake Events


The Modified Mercalli (MM) Intensity Scale is used in the United States. Based on Giuseppe Mercalli's Mercalli intensity scale of 1902, the modified 1931 scale is composed of increasing levels of intensity that range from observable quake impacts from light shaking to catastrophic destruction. Roman numerals report intensity.

An earthquake intensity scale consists of a series of critical responses, including people awakening, furniture movement, damage to chimneys, and destruction.
<table class="fullTable" width="100%"><thead><tr><th width="20%">Intensity</th>
<th width="20%">Shaking</th>
<th width="60%">Description/Damage</th>
</tr></thead><tbody><tr><td>I</td>
<td>Not Felt</td>
<td>Not felt except by a very few under especially favorable conditions.</td>
</tr><tr><td style="background-color: #DFE5F4; color: black">II</td>
<td>Weak</td>
<td>Felt only by a few persons at rest, especially on upper floors of buildings. Delicately suspended objects may swing.</td>
</tr><tr><td style="background-color: #9CDAE5; color: black">III</td>
<td>Weak</td>
<td>Felt quite noticeably by persons indoors, especially on upper floors of buildings. Many people do not recognize it as an earthquake. Standing motor cars may rock slightly. Vibration similar to the passing of a truck. Duration estimated.</td>
</tr><tr><td style="background-color: #99D6CC; color: black">IV</td>
<td>Light</td>
<td>Felt indoors by many, outdoors by few during the day. At night, some awakened. Dishes, windows, doors disturbed; walls make cracking sound. Sensation like heavy truck striking building. Standing motor cars rocked noticeably.</td>
</tr><tr><td style="background-color: #A4D177; color: black">V</td>
<td>Moderate</td>
<td>Felt by nearly everyone; many awakened. some dishes, windows broken. Unstable objects overturned. Pendulum clocks may stop.</td>
</tr><tr><td style="background-color: #F3EC56; color: black">VI</td>
<td>Strong</td>
<td>Felt by all, many frightened. Some heavy furniture moved; a few instances of fallen plaster. Damage slight.</td>
</tr><tr><td style="background-color: #FDC93F; color: black">VII</td>
<td>Very Strong</td>
<td>Damage negligible in buildings of good design and construction; slight to moderate in well-built ordinary structures; considerable damage in poorly built or badly designed structures; some chimneys broken.</td>
</tr><tr><td style="background-color: #F37033; color: black">VIII</td>
<td>Severe</td>
<td>Damage slight in specially designed structures; considerable damage in ordinary substantial buildings with partial collapse. Damage great in poorly built structures. Fall of chimneys, factory stacks, columns, monuments, walls. Heavy furniture overturned.</td>
</tr><tr><td style="background-color: #E92926; color: black">IX</td>
<td>Violent</td>
<td>Damage considerable in specially designed structures; well-designed frame structures thrown out of plumb. Damage great in substantial buildings, with partial collapse. Buildings shifted off foundations.</td>
</tr><tr><td style="background-color: #C62327; color: black">X</td>
<td>Extreme</td>
<td>Some well-built wooden structures destroyed; most masonry and frame structures destroyed with foundations. Rail bent.</td>
</tr></tbody></table>
   

Earthquake Magnitude Scale
Magnitude scales can be used to describe earthquakes so small that they are expressed in negative numbers. The scale also has no upper limit. Learn more about how we measure earthquake magnitude.


<table>
    <tr>
        <td>Magnitude</td>
        <td>Earthquake Effects</td>
    </tr>
    <tr>
        <td>2.5 or less</td>
        <td>Usually not felt, but can be recorded by seismograph.</td>
    </tr>
    <tr>
        <td>2.5 to 5.4</td>
        <td>Often felt, but only causes minor damage.</td>
    </tr>
    <tr>
        <td>5.5 to 6.0</td>
        <td>Slight damage to buildings and other structures.</td>
    </tr>
    <tr>
        <td>6.1 to 6.9</td>
        <td>May cause a lot of damage in very populated areas.</td>
    </tr>
    <tr>
        <td>7.0 to 7.9</td>
        <td>Major earthquake. Serious damage.</td>
    </tr>
    <tr>
        <td>8.0 or greater</td>
        <td>Great earthquake. Can totally destroy communities near the epicenter.</td>
    </tr>
</table>

<table class="tabular">
<tbody>
<tr valign="top">
<th id="t1">Magnitude</th>
<th id="t2">Typical Maximum<br>
Modified Mercalli Intensity</th>
</tr>
<tr>
<td headers="t1"><b>1.0 – 3.0</b></td>
<td headers="t2"><b>I</b></td>
</tr>
<tr>
<td headers="t1"><b>3.0 – 3.9</b></td>
<td headers="t2"><b>II – III</b></td>
</tr>
<tr>
<td headers="t1"><b>4.0 – 4.9</b></td>
<td headers="t2"><b>IV – V</b></td>
</tr>
<tr>
<td headers="t1"><b>5.0 – 5.9</b></td>
<td headers="t2"><b>VI – VII</b></td>
</tr>
<tr>
<td><b>6.0 – 6.9</b></td>
<td headers="t2"><b>VII – IX</b></td>
</tr>
<tr>
<td headers="t1"><b>7.0</b> and higher</td>
<td headers="t2"><b>VIII</b> or higher</td>
</tr>
</tbody>
</table>