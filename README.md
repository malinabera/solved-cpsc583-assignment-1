Download Link: https://assignmentchef.com/product/solved-cpsc583-assignment-1
<br>
In programming assignment 2, you will create a simple bar chart with your project data in D3.  You will also work with an existing tree visualization created with D3 and modify the D3 library to adjust the tree’s structure.

The goal of the assignment is to ensure you can create a simple visualization as well as to open the “black box” that is D3 and to learn that peeking into the library itself might be beneficial to understand how it works, to be able to better use D3, potentially modify it, and to think critically about what belongs in a library more broadly.

<h1>A) CREATING A SIMPLE CHART</h1>

In lectures and tutorials you have been given the basics of how to use D3.  Make use of this now to create a simple stacked bar chart from your project data submitted for the first part of the project.  You will use bar size for a quantitative property, a categorical to separate your data into bars, and your choice of either a different categorical or quantitative property to colour the bars. Key components:

<ol>

 <li>Load your data using D3’s CSV library</li>

 <li>Provide labelled axes using D3 scales to layout your axes</li>

 <li>Colours the bars and include a legend that provides the viewer with an explanation of the colour mapping</li>

 <li>Use hover events to provide the exact values associated with each bar</li>

 <li>This part of the assignment will be marked on how closely you are able to match the layout (position and orientation of the elements, you do not need to match the colour scheme, data, or fonts) of the chart</li>

</ol>







<h1>B) MODIFYING D3</h1>

D3 has a wealth of functionality, but how is this provided? Typically, we just use D3 without thinking about how it works internally. In this assignment, you are asked to work with D3’s tree layout. The tree layout in D3 produces tidy node-link diagrams of trees using the Reingold–Tilford “tidy” algorithm [1], improved to run in linear time by Buchheim et al. [2].

Your task is to modify how D3 creates a tree to produce a <em>visually distinct</em> tree compared to D3’s implementation. Run-time performance is not important for this assignment but your resulting tree should be noticeably different than the initial rendering. The task consists of the following steps.

<ul>

 <li>Take the provided code and make sure that it works. Easiest thing (which also helps in the next steps) is to create a new WebStorm project and add all three files to the project root. This should produce the following result in your browser:</li>

</ul>




<ul>

 <li>Using WebStorm, explore the code in index.html. <u>Do not change anything in this file!</u></li>

 <li>Using WebStorm, control-click on the tree call on line 41. This should take you to the “exports” statements in D3. Now control-click on the tree on the right side of the statement.</li>

 <li>Looking at the D3 code for a tree, try and make sense of what is going on. Making sure that you can easily revert to the original version, try to alter the behavior and observe the effects on the produced tree when doing a browser refresh.</li>

 <li>Consider which <em>visually distinct</em> change you would like to see happen in the produced output. This should alter the layout of the tree (position, orientation, or order as opposed to colours, labels, or sizes). Decide on one thing and write it down (you will put this in your hand-in).</li>

 <li>Now, attempt to create the <em>visually distinct</em> change that you decided on by only changing code in the D3 library. If you do not succeed in creating the planned change but did something else that created a <em>visually distinct</em> change, that is ok.</li>

</ul>

<h1>REFLECTION</h1>

The next steps are reflective and should be included in your hand-in.

<ul>

 <li>For Parts A &amp; B were you able to produce what you aimed for? Did you get something else that worked? Are you happy with the produced output? Write down your thoughts.</li>

 <li>In B you were asked to do your changes <u>in</u> the D3 library. Could you have done it without changing the library?</li>

</ul>

Would that have been better and why? Since you changed the behavior of the tree function, the original behavior is removed. Could the library offer both, and if so, then how? Write down your thoughts.