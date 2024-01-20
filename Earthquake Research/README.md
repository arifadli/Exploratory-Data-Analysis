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
   




