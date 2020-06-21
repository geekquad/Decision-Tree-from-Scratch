# Decision-Tree-from-Scratch
A decision tree is a flowchart-like tree structure where an internal node represents feature(or attribute), the branch represents a decision rule, and each leaf node represents the outcome. This flowchart-like structure helps us in decision making.

<img src="https://res.cloudinary.com/dyd911kmh/image/upload/f_auto,q_auto:best/v1545934190/1_r5ikdb.png">
Thiss why decision trees are easy to understand and interpret.
<p> <h3> Parameters: </h3> </p>
<ul>
  <li><b>min_samples_split (default value = 2)</b></li>
  nodes cannot be further seperated below this value. 
  <li><b> criterion : optional (default=”gini”)  </b></li>
  It controls how a Decision Tree decides where to split the data. 
  It is the measure of <b>impurity</b> in a bunch of examples. 
   This parameter allows us to use the different-different attribute selection measure. Supported criteria are “gini” for the Gini index and “entropy” for the information gain.
  <li> <b> splitter </b></li>
  This parameter allows us to choose the split strategy. Supported strategies are “best” to choose the best split and “random” to choose the best random split.
  </ul>
 <hr>                                                                                                 </hr>
<h3> Documentation of Decision Tree: </h3>
<a href="https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html">https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html</a>
<hr> </hr>
<h3> For Visualization </h3>
<p> Import the following libraries: </p>

```
from sklearn.tree import export_graphviz
from sklearn.externals.six import StringIO
from IPython.display import Image
import pydotplus
```
If the error **Graphviz executables not found** occurs, the run the following command:
```
import os
os.environ['PATH'] = os.environ['PATH']+';'+os.environ['CONDA_PREFIX']+r"\Library\bin\graphviz"
```
<p> <h3> Visulazization and Accuracy of the Tree using default parameters: </h3> </p>
<img src="https://github.com/geekquad/Decision-Tree-from-Scratch/blob/master/without_param_tune.png">
<h4> Accuracy : 0.66 </h4>
<p> <h3> Visulazization and Accuracy of the Tree after parameter tuning: </h3> </p>
<img src="https://github.com/geekquad/Decision-Tree-from-Scratch/blob/master/with_param_tune.png">
<h4> Accuracy : 0.77 </h4>
This pruned model is less complex, explainable, and easy to understand than the previous decision tree model plot.
                                                                                                
