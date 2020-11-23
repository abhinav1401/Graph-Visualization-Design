# Graph-Visualization-Design

<h3> Tools Used - Power BI and MS Excel </h3>

<img align="left" alt="PowerBI" width="29px" src="https://img.icons8.com/color/48/000000/power-bi.png"/>
<img align="left" alt="Excel" width="29px" src="https://img.icons8.com/fluent/48/000000/microsoft-excel-2019.png"/>

The aim of this assignment is to work with the given flight data to process and transform the data in order to design a graph visualization to satisfy a list of specific user’s requirements. In the design, it is required to select an appropriate graph layout method and to create a set of optimized graphical properties that 
are mapping to a set of data’s domain-specific attributes for better readability and understanding of the relational data structure as well as six data’s attributes. The data given is as follow:


<table class="tableizer-table">
<thead><tr class="tableizer-firstrow"><th>Air Space Class</th><th>From City</th><th>To City</th><th>Price</th><th>Aircraft Model</th><th>Engine Model</th></tr></thead><tbody>
 <tr><td>B</td><td>Sydeny</td><td>Melbourne</td><td>180</td><td>A330-203</td><td>CF6-80E142</td></tr>
 <tr><td>A</td><td>Sydeny</td><td>Brisbane</td><td>170</td><td>A330-202</td><td>CF6-80E142</td></tr>
 <tr><td>B</td><td>Sydeny</td><td>Canberra</td><td>120</td><td>B737-3B7</td><td>CFM56-3B1</td></tr>
 <tr><td>B</td><td>Canberra</td><td>Sydney</td><td>120</td><td>B737-476</td><td>CFM-56-3</td></tr>
 <tr><td>A</td><td>Sydeny</td><td>Newcastle</td><td>90</td><td>A320-232</td><td>V2527-5A</td></tr>
 <tr><td>A</td><td>Newcastle</td><td>Sydney</td><td>90</td><td>A320-232</td><td>V2527-5A</td></tr>
 <tr><td>B</td><td>Sydney</td><td>Broken Hill</td><td>130</td><td>A320-232</td><td>V2527-5A</td></tr>
 <tr><td>B</td><td>Broken Hill</td><td>Sydney</td><td>130</td><td>A320-232</td><td>V2527-5A</td></tr>
 <tr><td>C</td><td>Melbourne</td><td>Sydney</td><td>180</td><td>A330-243</td><td>772B-60</td></tr>
 <tr><td>B</td><td>Melbourne</td><td>Canberra</td><td>140</td><td>A320-232</td><td>V2527-5A</td></tr>
 <tr><td>B</td><td>Canberra</td><td>Melbourne</td><td>140</td><td>A320-232</td><td>V2527-5A</td></tr>
 <tr><td>A</td><td>Melbourne</td><td>Adelaide</td><td>175</td><td>B737-3B7</td><td>CFM56-3B1</td></tr>
 <tr><td>A</td><td>Melbourne</td><td>Hobart</td><td>130</td><td>A320-232</td><td>V2527-5A</td></tr>
 <tr><td>A</td><td>Melbourne</td><td>Bendigo</td><td>70</td><td>B717-200</td><td>Unknown</td></tr>
 <tr><td>A</td><td>Bendigo</td><td>Melbourne</td><td>70</td><td>B717-200</td><td>Unknown</td></tr>
 <tr><td>A</td><td>Melbourne</td><td>Launceston</td><td>100</td><td>B737-3B7</td><td>CFM56-3B1</td></tr>
 <tr><td>C</td><td>Adelaide</td><td>Melbourne</td><td>175</td><td>B737-3B7</td><td>CFM56-3B1</td></tr>
 <tr><td>C</td><td>Adelaide</td><td>Broken Hill</td><td>100</td><td>A320-232</td><td>V2527-5A</td></tr>
 <tr><td>C</td><td>Broken Hill</td><td>Adelaide</td><td>100</td><td>A320-232</td><td>V2527-5A</td></tr>
 <tr><td>D</td><td>Adelaide</td><td>Perth</td><td>220</td><td>A330-203</td><td>CF6-80E142 </td></tr>
 <tr><td>D</td><td>Adelaide</td><td>Darwin</td><td>230</td><td>A330-203</td><td>CF6-80E142 </td></tr>
 <tr><td>D</td><td>Darwin</td><td>Adelaide</td><td>230</td><td>A330-203</td><td>CF6-80E142 </td></tr>
 <tr><td>E</td><td>Darwin</td><td>Alice Springs</td><td>120</td><td>B737-476</td><td>CFM-56-3</td></tr>
 <tr><td>E</td><td>Alice Springs</td><td>Darwin</td><td>120</td><td>B737-476</td><td>CFM-56-3</td></tr>
 <tr><td>D</td><td>Perth</td><td>Adelaide</td><td>220</td><td>A330-203</td><td>CF6-80E142</td></tr>
 <tr><td>C</td><td>Perth</td><td>Albany</td><td>100</td><td>A320-232</td><td>V2527-5A</td></tr>
 <tr><td>C</td><td>Perth</td><td>Kalgoorlie</td><td>80</td><td>A320-232</td><td>V2527-5A</td></tr>
 <tr><td>C</td><td>Perth</td><td>Broome</td><td>90</td><td>A320-232</td><td>V2527-5A</td></tr>
 <tr><td>B</td><td>Albany</td><td>Perth</td><td>100</td><td>A320-232</td><td>V2527-5A</td></tr>
 <tr><td>C</td><td>Kalgoorlie</td><td>Perth</td><td>80</td><td>A320-232</td><td>V2527-5A</td></tr>
 <tr><td>B</td><td>Broome</td><td>Perth</td><td>90</td><td>B737-476</td><td>CFM-56-3</td></tr>
 <tr><td>B</td><td>Launceston</td><td>Melbourne</td><td>100</td><td>B737-476</td><td>CFM-56-3</td></tr>
 <tr><td>B</td><td>Launceston</td><td>Hobart</td><td>80</td><td>A320-232</td><td>V2527-5A</td></tr>
 <tr><td>A</td><td>Hobart</td><td>Melbourne</td><td>130</td><td>B737-3B7</td><td>CFM56-3B1</td></tr>
 <tr><td>A</td><td>Hobart</td><td>Launceston</td><td>80</td><td>A320-232</td><td>V2527-5A</td></tr>
 <tr><td>B</td><td>Brisbane</td><td>Sydney</td><td>170</td><td>A330-203</td><td>CF6-80E142</td></tr>
 <tr><td>A</td><td>Brisbane</td><td>Mt Isa</td><td>170</td><td>B737-3B7</td><td>CFM56-3B1</td></tr>
 <tr><td>A</td><td>Brisbane</td><td>Rockhampton</td><td>180</td><td>B737-3B7</td><td>CFM56-3B1</td></tr>
 <tr><td>A</td><td>Brisbane</td><td>Cairns</td><td>230</td><td>A330-203</td><td>CF6-80E142</td></tr>
 <tr><td>B</td><td>Brisbane</td><td>Darwin</td><td>240</td><td>A330-203</td><td>CF6-80E142</td></tr>
 <tr><td>A</td><td>Mt Isa</td><td>Brisbane</td><td>170</td><td>A330-202</td><td>CF6-80E142</td></tr>
 <tr><td>B</td><td>Rockhampton</td><td>Brisbane</td><td>180</td><td>A330-202</td><td>CF6-80E142</td></tr>
 <tr><td>A</td><td>Cairns</td><td>Brisbane</td><td>230</td><td>A330-203</td><td>CF6-80E142</td></tr>
 <tr><td>A</td><td>Darwin</td><td>Brisbane</td><td>240</td><td>A330-203</td><td>CF6-80E142</td></tr>
 <tr><td>B</td><td>Mt Isa</td><td>Darwin</td><td>120</td><td>B737-3B7</td><td>CFM56-3B1</td></tr>
 <tr><td>B</td><td>Darwin</td><td>Mt Isa</td><td>120</td><td>B737-3B7</td><td>CFM56-3B1</td></tr>
 <tr><td>B</td><td>Adelaide</td><td>Pt Augusta</td><td>50</td><td>B717-200</td><td>Unknown</td></tr>
 <tr><td>C</td><td>Pt Augusta</td><td>Adelaide</td><td>50</td><td>B717-200</td><td>Unknown</td></tr>
</tbody></table>

<h3> Solution </h3>

After processing and transforming the data, Directional Node-Link approach is selected as the graph visualization technique to represent the flights' data. Figure below shows the representation of flights data in a graphical manner. 

![alt text](https://github.com/abhinav1401/Graph-Visualization-Design/blob/main/Graph_Final.jpg)

It follows the basic properties of the node-link graph, where nodes represent the cities and the links between various node represent the flight path. Node-link approach was most suitable to represent the given data as the given data attributes can be easily represented by nodes and edges. <b>The repo contains .pbix files which can be directly loaded into PowerBI.</b> The transformed data is as follow:

<table class="tableizer-table">
<thead><tr class="tableizer-firstrow"><th>Air Space Class</th><th>Class Color</th><th>From City</th><th>Color</th><th>To City</th><th>Price</th><th>Aircraft Model</th><th>Aircraft Model Category</th><th>Engine Model</th></tr></thead><tbody>
 <tr><td>B</td><td>Blue</td><td>Sydeny</td><td>Light Blue</td><td>Melbourne</td><td>180</td><td>A330-203</td><td>category3</td><td>CF6-80E142</td></tr>
 <tr><td>A</td><td>Red</td><td>Sydeny</td><td>Light Blue</td><td>Brisbane</td><td>170</td><td>A330-202</td><td>category2</td><td>CF6-80E142</td></tr>
 <tr><td>B</td><td>Blue</td><td>Sydeny</td><td>Light Blue</td><td>Canberra</td><td>120</td><td>B737-3B7</td><td>category6</td><td>CFM56-3B1</td></tr>
 <tr><td>B</td><td>Blue</td><td>Canberra</td><td>Light Blue</td><td>Sydney</td><td>120</td><td>B737-476</td><td>category7</td><td>CFM-56-3</td></tr>
 <tr><td>A</td><td>Red</td><td>Sydeny</td><td>Light Blue</td><td>Newcastle</td><td>90</td><td>A320-232</td><td>category1</td><td>V2527-5A</td></tr>
 <tr><td>A</td><td>Red</td><td>Newcastle</td><td>Light Blue</td><td>Sydney</td><td>90</td><td>A320-232</td><td>category1</td><td>V2527-5A</td></tr>
 <tr><td>B</td><td>Blue</td><td>Sydney</td><td>Light Blue</td><td>Broken Hill</td><td>130</td><td>A320-232</td><td>category1</td><td>V2527-5A</td></tr>
 <tr><td>B</td><td>Blue</td><td>Broken Hill</td><td>Light Blue</td><td>Sydney</td><td>130</td><td>A320-232</td><td>category1</td><td>V2527-5A</td></tr>
 <tr><td>C</td><td>Green</td><td>Melbourne</td><td>Light Blue</td><td>Sydney</td><td>180</td><td>A330-243</td><td>category4</td><td>772B-60</td></tr>
 <tr><td>B</td><td>Blue</td><td>Melbourne</td><td>Light Blue</td><td>Canberra</td><td>140</td><td>A320-232</td><td>category1</td><td>V2527-5A</td></tr>
 <tr><td>B</td><td>Blue</td><td>Canberra</td><td>Light Blue</td><td>Melbourne</td><td>140</td><td>A320-232</td><td>category1</td><td>V2527-5A</td></tr>
 <tr><td>A</td><td>Red</td><td>Melbourne</td><td>Light Blue</td><td>Adelaide</td><td>175</td><td>B737-3B7</td><td>category6</td><td>CFM56-3B1</td></tr>
 <tr><td>A</td><td>Red</td><td>Melbourne</td><td>Light Blue</td><td>Hobart</td><td>130</td><td>A320-232</td><td>category1</td><td>V2527-5A</td></tr>
 <tr><td>A</td><td>Red</td><td>Melbourne</td><td>Light Blue</td><td>Bendigo</td><td>70</td><td>B717-200</td><td>category5</td><td>Unknown</td></tr>
 <tr><td>A</td><td>Red</td><td>Bendigo</td><td>Light Blue</td><td>Melbourne</td><td>70</td><td>B717-200</td><td>category5</td><td>Unknown</td></tr>
 <tr><td>A</td><td>Red</td><td>Melbourne</td><td>Light Blue</td><td>Launceston</td><td>100</td><td>B737-3B7</td><td>category6</td><td>CFM56-3B1</td></tr>
 <tr><td>C</td><td>Green</td><td>Adelaide</td><td>Light Blue</td><td>Melbourne</td><td>175</td><td>B737-3B7</td><td>category6</td><td>CFM56-3B1</td></tr>
 <tr><td>C</td><td>Green</td><td>Adelaide</td><td>Light Blue</td><td>Broken Hill</td><td>100</td><td>A320-232</td><td>category1</td><td>V2527-5A</td></tr>
 <tr><td>C</td><td>Green</td><td>Broken Hill</td><td>Light Blue</td><td>Adelaide</td><td>100</td><td>A320-232</td><td>category1</td><td>V2527-5A</td></tr>
 <tr><td>D</td><td>Black</td><td>Adelaide</td><td>Light Blue</td><td>Perth</td><td>220</td><td>A330-203</td><td>category3</td><td>CF6-80E142 </td></tr>
 <tr><td>D</td><td>Black</td><td>Adelaide</td><td>Light Blue</td><td>Darwin</td><td>230</td><td>A330-203</td><td>category3</td><td>CF6-80E142 </td></tr>
 <tr><td>D</td><td>Black</td><td>Darwin</td><td>Light Blue</td><td>Adelaide</td><td>230</td><td>A330-203</td><td>category3</td><td>CF6-80E142 </td></tr>
 <tr><td>E</td><td>Yellow</td><td>Darwin</td><td>Light Blue</td><td>Alice Springs</td><td>120</td><td>B737-476</td><td>category7</td><td>CFM-56-3</td></tr>
 <tr><td>E</td><td>Yellow</td><td>Alice Springs</td><td>Light Blue</td><td>Darwin</td><td>120</td><td>B737-476</td><td>category7</td><td>CFM-56-3</td></tr>
 <tr><td>D</td><td>Black</td><td>Perth</td><td>Light Blue</td><td>Adelaide</td><td>220</td><td>A330-203</td><td>category3</td><td>CF6-80E142</td></tr>
 <tr><td>C</td><td>Green</td><td>Perth</td><td>Light Blue</td><td>Albany</td><td>100</td><td>A320-232</td><td>category1</td><td>V2527-5A</td></tr>
 <tr><td>C</td><td>Green</td><td>Perth</td><td>Light Blue</td><td>Kalgoorlie</td><td>80</td><td>A320-232</td><td>category8</td><td>V2527-5A</td></tr>
 <tr><td>C</td><td>Green</td><td>Perth</td><td>Light Blue</td><td>Broome</td><td>90</td><td>A320-232</td><td>category9</td><td>V2527-5A</td></tr>
 <tr><td>B</td><td>Blue</td><td>Albany</td><td>Light Blue</td><td>Perth</td><td>100</td><td>A320-232</td><td>category1</td><td>V2527-5A</td></tr>
 <tr><td>C</td><td>Green</td><td>Kalgoorlie</td><td>Light Blue</td><td>Perth</td><td>80</td><td>A320-232</td><td>category8</td><td>V2527-5A</td></tr>
 <tr><td>B</td><td>Blue</td><td>Broome</td><td>Light Blue</td><td>Perth</td><td>90</td><td>B737-476</td><td>category7</td><td>CFM-56-3</td></tr>
 <tr><td>B</td><td>Blue</td><td>Launceston</td><td>Light Blue</td><td>Melbourne</td><td>100</td><td>B737-476</td><td>category7</td><td>CFM-56-3</td></tr>
 <tr><td>B</td><td>Blue</td><td>Launceston</td><td>Light Blue</td><td>Hobart</td><td>80</td><td>A320-232</td><td>category8</td><td>V2527-5A</td></tr>
 <tr><td>A</td><td>Red</td><td>Hobart</td><td>Light Blue</td><td>Melbourne</td><td>130</td><td>B737-3B7</td><td>category6</td><td>CFM56-3B1</td></tr>
 <tr><td>A</td><td>Red</td><td>Hobart</td><td>Light Blue</td><td>Launceston</td><td>80</td><td>A320-232</td><td>category8</td><td>V2527-5A</td></tr>
 <tr><td>B</td><td>Blue</td><td>Brisbane</td><td>Light Blue</td><td>Sydney</td><td>170</td><td>A330-203</td><td>category3</td><td>CF6-80E142</td></tr>
 <tr><td>A</td><td>Red</td><td>Brisbane</td><td>Light Blue</td><td>Mt Isa</td><td>170</td><td>B737-3B7</td><td>category6</td><td>CFM56-3B1</td></tr>
 <tr><td>A</td><td>Red</td><td>Brisbane</td><td>Light Blue</td><td>Rockhampton</td><td>180</td><td>B737-3B7</td><td>category6</td><td>CFM56-3B1</td></tr>
 <tr><td>A</td><td>Red</td><td>Brisbane</td><td>Light Blue</td><td>Cairns</td><td>230</td><td>A330-203</td><td>category3</td><td>CF6-80E142</td></tr>
 <tr><td>B</td><td>Blue</td><td>Brisbane</td><td>Light Blue</td><td>Darwin</td><td>240</td><td>A330-203</td><td>category3</td><td>CF6-80E142</td></tr>
 <tr><td>A</td><td>Red</td><td>Mt Isa</td><td>Light Blue</td><td>Brisbane</td><td>170</td><td>A330-202</td><td>category3</td><td>CF6-80E142</td></tr>
 <tr><td>B</td><td>Blue</td><td>Rockhampton</td><td>Light Blue</td><td>Brisbane</td><td>180</td><td>A330-202</td><td>category3</td><td>CF6-80E142</td></tr>
 <tr><td>A</td><td>Red</td><td>Cairns</td><td>Light Blue</td><td>Brisbane</td><td>230</td><td>A330-203</td><td>category3</td><td>CF6-80E142</td></tr>
 <tr><td>A</td><td>Red</td><td>Darwin</td><td>Light Blue</td><td>Brisbane</td><td>240</td><td>A330-203</td><td>category3</td><td>CF6-80E142</td></tr>
 <tr><td>B</td><td>Blue</td><td>Mt Isa</td><td>Light Blue</td><td>Darwin</td><td>120</td><td>B737-3B7</td><td>category6</td><td>CFM56-3B1</td></tr>
 <tr><td>B</td><td>Blue</td><td>Darwin</td><td>Light Blue</td><td>Mt Isa</td><td>120</td><td>B737-3B7</td><td>category6</td><td>CFM56-3B1</td></tr>
 <tr><td>B</td><td>BLue</td><td>Adelaide</td><td>Light Blue</td><td>Pt Augusta</td><td>50</td><td>B717-200</td><td>category5</td><td>Unknown</td></tr>
 <tr><td>C</td><td>Green</td><td>Pt Augusta</td><td>Light Blue</td><td>Adelaide</td><td>50</td><td>B717-200</td><td>category5</td><td>Unknown</td></tr>
</tbody></table>
