![DecisionTree](https://github.com/user-attachments/assets/e56db403-e73f-422a-8653-af8e55d27c69)# 🛍️ Shopping Habits Predictor with ML
## Project Overview
This project presents a simple machine learning approach to predicting the shopping habits based on age and gender. Trained on a labeled dataset, the model is designed to make predictions for previously unseen demographic combinations. The project is built using the pandas and scikit-learn libraries. 

### Data Sources
The dataset used for model training was created by the author. It includes synthetic entries with age, gender, and corresponding music genre preferences.

### Tools
- Jupyter Notebook
- Python 
  - pandas - Data Analysis
  - sklearn - Model training/testing, prediction and basic visualization
 
### Data Cleaning
As the dataset was synthetically created by the author with a limited number of rows and columns, no additional data cleaning was necessary.

## Machine Learning
### Creating Model
A Decision Tree Classifier from scikit-learn was used to train the model on a labeled dataset. The input features were age and gender, while the target (output) was shopping habits. Since the dataset does not include every possible age and gender combination, we use the trained model to predict shopping habits for new, unseen inputs.
### Measure Model Accuracy
The dataset was split into training and test sets using <code style="color : name_color">train_test_split</code>. To evaluate the model’s performance, we used the <code style="color : name_color">accuracy_score</code> function from <code style="color : name_color">sklearn.metrics</code>. The accuracy score may vary slightly with each execution, as the data is randomly split by default.

### Persisting the Model
The trained model was saved using the <code style="color : name_color">joblib</code> library for future use. This step allows us to make predictions without retraining the model.
### Visualizing the Desicion Tree
The structure of the trained decision tree was visualized using VSC with Graphviz Interactive Preview extension <img width="541" height="148" alt="Screenshot 2025-07-19 at 3 14 31 PM" src="https://github.com/user-attachments/assets/4d92f215-372c-418a-b015-36b2aa4c025d" />

This visualization helps illustrate the decision-making process of the model. At each node, the tree asks a question based on the input features (in our case, age or gender). If the condition is true, the model follows one branch, if false, it follows the other. The process continues until the model reaches a leaf node, or, in other words, the final predicted outcome.

## Final Result
![Uploadin<?xml version="1.0" standalone="no"?>
<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="915pt" height="467pt" viewBox="0.00 0.00 915.09 467.20">
<g id="graph0" class="graph" transform="translate(4,463.20001220703125) scale(1)" data-name="Tree">

<polygon fill="white" stroke="none" points="-4,4 -4,-463.2 911.09,-463.2 911.09,4 -4,4" style=""/>
<!-- 0 -->
<g id="node1" class="node" pointer-events="visible" data-name="0">

<path fill="none" stroke="black" d="M426.26,-459.2C426.26,-459.2 268.55,-459.2 268.55,-459.2 262.55,-459.2 256.55,-453.2 256.55,-447.2 256.55,-447.2 256.55,-379.2 256.55,-379.2 256.55,-373.2 262.55,-367.2 268.55,-367.2 268.55,-367.2 426.26,-367.2 426.26,-367.2 432.26,-367.2 438.26,-373.2 438.26,-379.2 438.26,-379.2 438.26,-447.2 438.26,-447.2 438.26,-453.2 432.26,-459.2 426.26,-459.2" style=""/>
<text text-anchor="middle" x="347.41" y="-442.6" font-family="Helvetica,sans-Serif" font-size="14.00" style="">age &lt;= 31.0</text>
<text text-anchor="middle" x="347.41" y="-425.8" font-family="Helvetica,sans-Serif" font-size="14.00" style="">gini = 0.833</text>
<text text-anchor="middle" x="347.41" y="-409" font-family="Helvetica,sans-Serif" font-size="14.00" style="">samples = 18</text>
<text text-anchor="middle" x="347.41" y="-392.2" font-family="Helvetica,sans-Serif" font-size="14.00" style="">value = [3, 3, 3, 3, 3, 3]</text>
<text text-anchor="middle" x="347.41" y="-375.4" font-family="Helvetica,sans-Serif" font-size="14.00" style="">class = Necessity Shopper</text>
</g>
<!-- 1 -->
<g id="node2" class="node" pointer-events="visible" data-name="1">

<path fill="none" stroke="black" d="M320.72,-331.2C320.72,-331.2 186.09,-331.2 186.09,-331.2 180.09,-331.2 174.09,-325.2 174.09,-319.2 174.09,-319.2 174.09,-251.2 174.09,-251.2 174.09,-245.2 180.09,-239.2 186.09,-239.2 186.09,-239.2 320.72,-239.2 320.72,-239.2 326.72,-239.2 332.72,-245.2 332.72,-251.2 332.72,-251.2 332.72,-319.2 332.72,-319.2 332.72,-325.2 326.72,-331.2 320.72,-331.2" style=""/>
<text text-anchor="middle" x="253.41" y="-314.6" font-family="Helvetica,sans-Serif" font-size="14.00" style="">gender &lt;= 0.5</text>
<text text-anchor="middle" x="253.41" y="-297.8" font-family="Helvetica,sans-Serif" font-size="14.00" style="">gini = 0.5</text>
<text text-anchor="middle" x="253.41" y="-281" font-family="Helvetica,sans-Serif" font-size="14.00" style="">samples = 6</text>
<text text-anchor="middle" x="253.41" y="-264.2" font-family="Helvetica,sans-Serif" font-size="14.00" style="">value = [0, 0, 0, 3, 0, 3]</text>
<text text-anchor="middle" x="253.41" y="-247.4" font-family="Helvetica,sans-Serif" font-size="14.00" style="">class = Tech Buyer</text>
</g>
<!-- 0&#45;&gt;1 -->
<g id="edge1" class="edge" data-name="0-&gt;1">

<path fill="none" stroke="black" d="M313.47,-366.71C307.15,-358.24 300.48,-349.3 293.98,-340.59" style=""/>
<polygon fill="black" stroke="black" points="296.98,-338.76 288.2,-332.84 291.37,-342.94 296.98,-338.76" style=""/>
<text text-anchor="middle" x="283.7" y="-352.16" font-family="Helvetica,sans-Serif" font-size="14.00" style="">True</text>
</g>
<!-- 4 -->
<g id="node5" class="node" pointer-events="visible" data-name="4">

<path fill="none" stroke="black" d="M520.26,-331.2C520.26,-331.2 362.55,-331.2 362.55,-331.2 356.55,-331.2 350.55,-325.2 350.55,-319.2 350.55,-319.2 350.55,-251.2 350.55,-251.2 350.55,-245.2 356.55,-239.2 362.55,-239.2 362.55,-239.2 520.26,-239.2 520.26,-239.2 526.26,-239.2 532.26,-245.2 532.26,-251.2 532.26,-251.2 532.26,-319.2 532.26,-319.2 532.26,-325.2 526.26,-331.2 520.26,-331.2" style=""/>
<text text-anchor="middle" x="441.41" y="-314.6" font-family="Helvetica,sans-Serif" font-size="14.00" style="">gender &lt;= 0.5</text>
<text text-anchor="middle" x="441.41" y="-297.8" font-family="Helvetica,sans-Serif" font-size="14.00" style="">gini = 0.75</text>
<text text-anchor="middle" x="441.41" y="-281" font-family="Helvetica,sans-Serif" font-size="14.00" style="">samples = 12</text>
<text text-anchor="middle" x="441.41" y="-264.2" font-family="Helvetica,sans-Serif" font-size="14.00" style="">value = [3, 3, 3, 0, 3, 0]</text>
<text text-anchor="middle" x="441.41" y="-247.4" font-family="Helvetica,sans-Serif" font-size="14.00" style="">class = Necessity Shopper</text>
</g>
<!-- 0&#45;&gt;4 -->
<g id="edge4" class="edge" data-name="0-&gt;4">

<path fill="none" stroke="black" d="M381.34,-366.71C387.67,-358.24 394.33,-349.3 400.83,-340.59" style=""/>
<polygon fill="black" stroke="black" points="403.44,-342.94 406.62,-332.84 397.83,-338.76 403.44,-342.94" style=""/>
<text text-anchor="middle" x="411.12" y="-352.16" font-family="Helvetica,sans-Serif" font-size="14.00" style="">False</text>
</g>
<!-- 2 -->
<g id="node3" class="node" pointer-events="visible" data-name="2">

<path fill="none" stroke="black" d="M146.72,-194.9C146.72,-194.9 12.09,-194.9 12.09,-194.9 6.09,-194.9 0.09,-188.9 0.09,-182.9 0.09,-182.9 0.09,-131.5 0.09,-131.5 0.09,-125.5 6.09,-119.5 12.09,-119.5 12.09,-119.5 146.72,-119.5 146.72,-119.5 152.72,-119.5 158.72,-125.5 158.72,-131.5 158.72,-131.5 158.72,-182.9 158.72,-182.9 158.72,-188.9 152.72,-194.9 146.72,-194.9" style=""/>
<text text-anchor="middle" x="79.41" y="-178.2" font-family="Helvetica,sans-Serif" font-size="14.00" style="">gini = 0.0</text>
<text text-anchor="middle" x="79.41" y="-161.4" font-family="Helvetica,sans-Serif" font-size="14.00" style="">samples = 3</text>
<text text-anchor="middle" x="79.41" y="-144.6" font-family="Helvetica,sans-Serif" font-size="14.00" style="">value = [0, 0, 0, 0, 0, 3]</text>
<text text-anchor="middle" x="79.41" y="-127.8" font-family="Helvetica,sans-Serif" font-size="14.00" style="">class = Trend Shopper</text>
</g>
<!-- 1&#45;&gt;2 -->
<g id="edge2" class="edge" data-name="1-&gt;2">

<path fill="none" stroke="black" d="M190.59,-238.71C174,-226.7 156.13,-213.76 139.68,-201.85" style=""/>
<polygon fill="black" stroke="black" points="142.08,-199.26 131.93,-196.23 137.97,-204.93 142.08,-199.26" style=""/>
</g>
<!-- 3 -->
<g id="node4" class="node" pointer-events="visible" data-name="3">

<path fill="none" stroke="black" d="M323.72,-194.9C323.72,-194.9 189.09,-194.9 189.09,-194.9 183.09,-194.9 177.09,-188.9 177.09,-182.9 177.09,-182.9 177.09,-131.5 177.09,-131.5 177.09,-125.5 183.09,-119.5 189.09,-119.5 189.09,-119.5 323.72,-119.5 323.72,-119.5 329.72,-119.5 335.72,-125.5 335.72,-131.5 335.72,-131.5 335.72,-182.9 335.72,-182.9 335.72,-188.9 329.72,-194.9 323.72,-194.9" style=""/>
<text text-anchor="middle" x="256.41" y="-178.2" font-family="Helvetica,sans-Serif" font-size="14.00" style="">gini = 0.0</text>
<text text-anchor="middle" x="256.41" y="-161.4" font-family="Helvetica,sans-Serif" font-size="14.00" style="">samples = 3</text>
<text text-anchor="middle" x="256.41" y="-144.6" font-family="Helvetica,sans-Serif" font-size="14.00" style="">value = [0, 0, 0, 3, 0, 0]</text>
<text text-anchor="middle" x="256.41" y="-127.8" font-family="Helvetica,sans-Serif" font-size="14.00" style="">class = Tech Buyer</text>
</g>
<!-- 1&#45;&gt;3 -->
<g id="edge3" class="edge" data-name="1-&gt;3">

<path fill="none" stroke="black" d="M254.49,-238.71C254.74,-228.25 255.01,-217.1 255.26,-206.53" style=""/>
<polygon fill="black" stroke="black" points="258.75,-206.94 255.49,-196.86 251.75,-206.77 258.75,-206.94" style=""/>
</g>
<!-- 5 -->
<g id="node6" class="node" pointer-events="visible" data-name="5">

<path fill="none" stroke="black" d="M505.72,-203.2C505.72,-203.2 371.09,-203.2 371.09,-203.2 365.09,-203.2 359.09,-197.2 359.09,-191.2 359.09,-191.2 359.09,-123.2 359.09,-123.2 359.09,-117.2 365.09,-111.2 371.09,-111.2 371.09,-111.2 505.72,-111.2 505.72,-111.2 511.72,-111.2 517.72,-117.2 517.72,-123.2 517.72,-123.2 517.72,-191.2 517.72,-191.2 517.72,-197.2 511.72,-203.2 505.72,-203.2" style=""/>
<text text-anchor="middle" x="438.41" y="-186.6" font-family="Helvetica,sans-Serif" font-size="14.00" style="">age &lt;= 45.0</text>
<text text-anchor="middle" x="438.41" y="-169.8" font-family="Helvetica,sans-Serif" font-size="14.00" style="">gini = 0.5</text>
<text text-anchor="middle" x="438.41" y="-153" font-family="Helvetica,sans-Serif" font-size="14.00" style="">samples = 6</text>
<text text-anchor="middle" x="438.41" y="-136.2" font-family="Helvetica,sans-Serif" font-size="14.00" style="">value = [0, 3, 0, 0, 3, 0]</text>
<text text-anchor="middle" x="438.41" y="-119.4" font-family="Helvetica,sans-Serif" font-size="14.00" style="">class = Planner</text>
</g>
<!-- 4&#45;&gt;5 -->
<g id="edge5" class="edge" data-name="4-&gt;5">

<path fill="none" stroke="black" d="M440.33,-238.71C440.14,-231.04 439.95,-222.99 439.76,-215.07" style=""/>
<polygon fill="black" stroke="black" points="443.26,-215.05 439.53,-205.14 436.26,-215.22 443.26,-215.05" style=""/>
</g>
<!-- 8 -->
<g id="node9" class="node" pointer-events="visible" data-name="8">

<path fill="none" stroke="black" d="M707.26,-203.2C707.26,-203.2 549.55,-203.2 549.55,-203.2 543.55,-203.2 537.55,-197.2 537.55,-191.2 537.55,-191.2 537.55,-123.2 537.55,-123.2 537.55,-117.2 543.55,-111.2 549.55,-111.2 549.55,-111.2 707.26,-111.2 707.26,-111.2 713.26,-111.2 719.26,-117.2 719.26,-123.2 719.26,-123.2 719.26,-191.2 719.26,-191.2 719.26,-197.2 713.26,-203.2 707.26,-203.2" style=""/>
<text text-anchor="middle" x="628.41" y="-186.6" font-family="Helvetica,sans-Serif" font-size="14.00" style="">age &lt;= 43.5</text>
<text text-anchor="middle" x="628.41" y="-169.8" font-family="Helvetica,sans-Serif" font-size="14.00" style="">gini = 0.5</text>
<text text-anchor="middle" x="628.41" y="-153" font-family="Helvetica,sans-Serif" font-size="14.00" style="">samples = 6</text>
<text text-anchor="middle" x="628.41" y="-136.2" font-family="Helvetica,sans-Serif" font-size="14.00" style="">value = [3, 0, 3, 0, 0, 0]</text>
<text text-anchor="middle" x="628.41" y="-119.4" font-family="Helvetica,sans-Serif" font-size="14.00" style="">class = Necessity Shopper</text>
</g>
<!-- 4&#45;&gt;8 -->
<g id="edge8" class="edge" data-name="4-&gt;8">

<path fill="none" stroke="black" d="M508.92,-238.71C522.82,-229.34 537.56,-219.41 551.76,-209.85" style=""/>
<polygon fill="black" stroke="black" points="553.4,-212.96 559.74,-204.47 549.49,-207.15 553.4,-212.96" style=""/>
</g>
<!-- 6 -->
<g id="node7" class="node" pointer-events="visible" data-name="6">

<path fill="none" stroke="black" d="M315.72,-75.3C315.72,-75.3 181.09,-75.3 181.09,-75.3 175.09,-75.3 169.09,-69.3 169.09,-63.3 169.09,-63.3 169.09,-11.9 169.09,-11.9 169.09,-5.9 175.09,0.1 181.09,0.1 181.09,0.1 315.72,0.1 315.72,0.1 321.72,0.1 327.72,-5.9 327.72,-11.9 327.72,-11.9 327.72,-63.3 327.72,-63.3 327.72,-69.3 321.72,-75.3 315.72,-75.3" style=""/>
<text text-anchor="middle" x="248.41" y="-58.6" font-family="Helvetica,sans-Serif" font-size="14.00" style="">gini = 0.0</text>
<text text-anchor="middle" x="248.41" y="-41.8" font-family="Helvetica,sans-Serif" font-size="14.00" style="">samples = 3</text>
<text text-anchor="middle" x="248.41" y="-25" font-family="Helvetica,sans-Serif" font-size="14.00" style="">value = [0, 3, 0, 0, 0, 0]</text>
<text text-anchor="middle" x="248.41" y="-8.2" font-family="Helvetica,sans-Serif" font-size="14.00" style="">class = Planner</text>
</g>
<!-- 5&#45;&gt;6 -->
<g id="edge6" class="edge" data-name="5-&gt;6">

<path fill="none" stroke="black" d="M364.95,-110.73C349.47,-101.15 333.18,-91.07 317.86,-81.59" style=""/>
<polygon fill="black" stroke="black" points="320.09,-78.85 309.74,-76.56 316.4,-84.8 320.09,-78.85" style=""/>
</g>
<!-- 7 -->
<g id="node8" class="node" pointer-events="visible" data-name="7">

<path fill="none" stroke="black" d="M519.45,-75.3C519.45,-75.3 357.37,-75.3 357.37,-75.3 351.37,-75.3 345.37,-69.3 345.37,-63.3 345.37,-63.3 345.37,-11.9 345.37,-11.9 345.37,-5.9 351.37,0.1 357.37,0.1 357.37,0.1 519.45,0.1 519.45,0.1 525.45,0.1 531.45,-5.9 531.45,-11.9 531.45,-11.9 531.45,-63.3 531.45,-63.3 531.45,-69.3 525.45,-75.3 519.45,-75.3" style=""/>
<text text-anchor="middle" x="438.41" y="-58.6" font-family="Helvetica,sans-Serif" font-size="14.00" style="">gini = 0.0</text>
<text text-anchor="middle" x="438.41" y="-41.8" font-family="Helvetica,sans-Serif" font-size="14.00" style="">samples = 3</text>
<text text-anchor="middle" x="438.41" y="-25" font-family="Helvetica,sans-Serif" font-size="14.00" style="">value = [0, 0, 0, 0, 3, 0]</text>
<text text-anchor="middle" x="438.41" y="-8.2" font-family="Helvetica,sans-Serif" font-size="14.00" style="">class = Traditional Shopper</text>
</g>
<!-- 5&#45;&gt;7 -->
<g id="edge7" class="edge" data-name="5-&gt;7">

<path fill="none" stroke="black" d="M438.41,-110.73C438.41,-102.92 438.41,-94.77 438.41,-86.88" style=""/>
<polygon fill="black" stroke="black" points="441.91,-87.09 438.41,-77.09 434.91,-87.09 441.91,-87.09" style=""/>
</g>
<!-- 9 -->
<g id="node10" class="node" pointer-events="visible" data-name="9">

<path fill="none" stroke="black" d="M695.72,-75.3C695.72,-75.3 561.09,-75.3 561.09,-75.3 555.09,-75.3 549.09,-69.3 549.09,-63.3 549.09,-63.3 549.09,-11.9 549.09,-11.9 549.09,-5.9 555.09,0.1 561.09,0.1 561.09,0.1 695.72,0.1 695.72,0.1 701.72,0.1 707.72,-5.9 707.72,-11.9 707.72,-11.9 707.72,-63.3 707.72,-63.3 707.72,-69.3 701.72,-75.3 695.72,-75.3" style=""/>
<text text-anchor="middle" x="628.41" y="-58.6" font-family="Helvetica,sans-Serif" font-size="14.00" style="">gini = 0.0</text>
<text text-anchor="middle" x="628.41" y="-41.8" font-family="Helvetica,sans-Serif" font-size="14.00" style="">samples = 3</text>
<text text-anchor="middle" x="628.41" y="-25" font-family="Helvetica,sans-Serif" font-size="14.00" style="">value = [0, 0, 3, 0, 0, 0]</text>
<text text-anchor="middle" x="628.41" y="-8.2" font-family="Helvetica,sans-Serif" font-size="14.00" style="">class = Practical Buyer</text>
</g>
<!-- 8&#45;&gt;9 -->
<g id="edge9" class="edge" data-name="8-&gt;9">

<path fill="none" stroke="black" d="M628.41,-110.73C628.41,-102.92 628.41,-94.77 628.41,-86.88" style=""/>
<polygon fill="black" stroke="black" points="631.91,-87.09 628.41,-77.09 624.91,-87.09 631.91,-87.09" style=""/>
</g>
<!-- 10 -->
<g id="node11" class="node" pointer-events="visible" data-name="10">

<path fill="none" stroke="black" d="M895.26,-75.3C895.26,-75.3 737.55,-75.3 737.55,-75.3 731.55,-75.3 725.55,-69.3 725.55,-63.3 725.55,-63.3 725.55,-11.9 725.55,-11.9 725.55,-5.9 731.55,0.1 737.55,0.1 737.55,0.1 895.26,0.1 895.26,0.1 901.26,0.1 907.26,-5.9 907.26,-11.9 907.26,-11.9 907.26,-63.3 907.26,-63.3 907.26,-69.3 901.26,-75.3 895.26,-75.3" style=""/>
<text text-anchor="middle" x="816.41" y="-58.6" font-family="Helvetica,sans-Serif" font-size="14.00" style="">gini = 0.0</text>
<text text-anchor="middle" x="816.41" y="-41.8" font-family="Helvetica,sans-Serif" font-size="14.00" style="">samples = 3</text>
<text text-anchor="middle" x="816.41" y="-25" font-family="Helvetica,sans-Serif" font-size="14.00" style="">value = [3, 0, 0, 0, 0, 0]</text>
<text text-anchor="middle" x="816.41" y="-8.2" font-family="Helvetica,sans-Serif" font-size="14.00" style="">class = Necessity Shopper</text>
</g>
<!-- 8&#45;&gt;10 -->
<g id="edge10" class="edge" data-name="8-&gt;10">

<path fill="none" stroke="black" d="M701.09,-110.73C716.27,-101.24 732.22,-91.26 747.26,-81.85" style=""/>
<polygon fill="black" stroke="black" points="749.09,-84.84 755.71,-76.57 745.38,-78.9 749.09,-84.84" style=""/>
</g>
</g>
</svg>g DecisionTree.svg…]()

