# cs540-homework-7--clustering-solved
**TO GET THIS SOLUTION VISIT:** [CS540 Homework 7- Clustering Solved](https://www.ankitcodinghub.com/product/cs540-hw7-clustering-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;117940&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS540  Homework 7- Clustering Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Assignment Goals

Implement hierarchical clustering Process fun real-world data

Summary

Using the publicly available Pokemon stats, you’ll be performing clustering on these stats. Each

Pokemon is defined by a row in the data set. Because there are various ways to characterize how strong a Pokemon is, it is often desirable to convert a raw stats sheet into a shorter feature vector. For this assignment, you will represent a Pokemon’s strength by two numbers: “x” and “y”. “x” will represent the Pokemon’s total offensive strength, which is defined by Attack + Sp. Atk + Speed. Similarly, “y” will represent the Pokemon’s total defensive strength, which is defined by Defense + Sp. Def + HP. After each Pokemon becomes that two-dimensional feature vector, you will cluster the first 20 Pokemon with hierarchical agglomerative clustering (HAC).

Program Specification

Download the data in CSV format: Pokemon.csv

Write the following Python functions:

1. load_data(filepath) — takes in a string with a path to a CSV file formatted as in the link above, and returns the first 20 data points (without the Generation and Legendary columns but retaining all other columns) in a single structure.

2. calculate_x_y(stats) — takes in one row from the data loaded from the previous function, calculates the corresponding x, y values for that Pokemon as specified above, and returns them in a single structure.

3. hac(dataset) — performs single linkage hierarchical agglomerative clustering on the Pokemon with the (x,y) feature representation, and returns a data structure representing the clustering.

Load Data

Read in the file specified in the argument (the DictReader from Python’s csv module

(https://docs.python.org/3/library/csv.html#csv.DictReader) will be of use) and return a list of dictionaries, where each row in the dataset is a dictionary with the column headers as keys and the row elements as values. These dictionaries should not include the Generation and Legendary columns, as we will not be using them in this program. Also, you only should have the first 20 Pokemon in this structure. Note the first 20 refers to row 1 through row 20. Lastly, make sure to convert columns with numerical data to int in this method (e.g. HP, Attack, etc).

Calculate Feature Values

This function takes in the data from a single row of the raw dataset as read in the previous function (i.e. a single dictionary, without the Generation and Legendary values but retaining all other columns). This function should return the x, y values in a tuple, formatted as (x, y) .

Perform HAC

For this function, we would like you to mimic the behavior of SciPy’s HAC function

Using single linkage, perform the hierarchical agglomerative clustering algorithm as detailed on slide

42 of this presentation (https://happyharrycn.github.io/CS540-

Fall20/lectures/introML_hierarchical_clustering.pdf) . Use a standard Euclidean distance function for calculating the distance between two points.

Output: An (m-1) by 4 matrix Z . At the i-th iteration, clusters with indices Z[i, 0] and Z[i, 1] are combined to form cluster m + i. A cluster with an index less than m corresponds to one of the m original observations. The distance between clusters Z[i, 0] and Z[i, 1] is given by Z[i, 2] . The fourth value Z[i, 3] represents the number of original observations in the newly formed cluster.

That is:

Number each of your starting data points from 0 to m-1. These are their original cluster numbers.

Create an (m-1)x4 array or list. Iterate through the list row by row.

For each row, determine which two clusters you will merge and put their numbers into the first and second elements of the row. The first point listed should be the smaller of the two cluster indexes.

The single-linkage distance between the two clusters goes into the third element of the row. The total number of points in the cluster goes into the fourth element.

If you merge a cluster containing more than one data point, its number (for the first or second element of the row) is given by m+the row index in which the cluster was created.

Before returning the data structure, convert it into a NumPy matrix.

If you follow these guidelines for input and output, your result should match the result of scipy.cluster.hierarchy.linkage() and you can use that function to verify your results. Be aware that this

function does not contain code to filter NaN values, so this filtering should be performed before calling the function.

Tie Breaking

In the event that there are multiple pairs of points with equal distance for the next cluster:

Given a set of pairs with equal distance {(xi, xj)} where i &lt; j, we prefer the pair with the smallest first cluster index i. If there are still ties (xi, xj), … (xi, xk) where i is that smallest first index, we prefer the pair with the smallest second cluster index.

Submission Notes

Please submit your files in a zip file named hw7_&lt;netid&gt;.zip, where you replace &lt;netid&gt; with your netID (your wisc.edu login). Inside your zip file, there should be only one file named: pokemon_stats.py. Do not submit a Jupyter notebook .ipynb file.

All code should be contained in functions or under a

check so that it will not run if your code is imported to another program.

Be sure to remove all debugging output before submission. Failure to remove debugging output will be penalized (10pts).

Changelog

Updated to look at only the first 20 Pokemon

HW7

Criteria Ratings Pts

load_data() returns a list of dictionaries 10.0 pts

load_data() result does not include Generation/Legendary columns 10.0 pts

load_data() contains correct values from input csv 10.0 pts

calculate_x_y() returns a single two-element tuple 10.0 pts

calculate_x_y() return values match expected outputs 20.0 to &gt;0.0 pts

No

hac() returns an (m-1)*4 array, matrix, or list where m = the number of non-NaN Pokemon 10.0 pts

the third column of the hac() return array is strictly increasing 10.0 pts

hac() tie-breaking conforms to stated protocols 10.0 pts

hac() return value matches expected outputs 10.0 to &gt;0.0 pts

No
