# Decision-Tree

## Introduction

Over time, a large number of methods for data analysis have been developed, which are mainly based on statistical techniques. However, as the information stored grows considerably, traditional statistical methods have begun to face problems of efficiency and scalability. Since most of this information is historical and comes from various sources, the imminent need to seek alternative methods for the analysis of this type of data seems clear, and from them, to be able to obtain relevant and non-explicit information. In most cases, the analysis and interpretation of the data is done manually, that is, the specialist analyzes and prepares a report or hypothesis that reflects the trends or patterns of the same, in order to present his conclusions and from They can make important and meaningful decisions. As can be seen, this process is slow, expensive and highly subjective; in fact, manual analysis is impractical in situations where the volume of data grows exponentially, since the large amount of data exceeds the human capacity to understand it without the help of a suitable tool. Therefore, in most cases, important decisions are made not from the data, but from the intuition and experience of the experts, since they lack suitable tools to support them.
Decision trees are a classification model used in artificial intelligence, whose main characteristic is its visual contribution to decision making.ID3, Iterative Dichotomiser 3 is a decision tree learning algorithm used to classify decisions. objects with the iterative inductive approach. In this algorithm the top-down approach is used. The top node is called the root node and the others are leaf nodes. So it is a traversal from the root node to the leaf nodes. Each node requires some test on the attributes that decide the level of the leaf nodes. These decision trees are mainly used for decision making[1].

## 2. Theoretical Framework

Decision Tree is a machine learning algorithm used for data classification and predictive analytics. Decision learning algorithms guarantee decision trees from training data to solve classification and regression problems. Basically, they are used as predictive models to predict the value of a target variable by learning simple decision rules inferred from the characteristics of the data. These rules are often in the form of if-then statements. Then, the information obtained is used to decide which features to split in each configuration in the construction of the tree.

### 2.1 ID3

The Iterative Dichotomiser 3 (ID3) decision tree algorithm was designed by Quinlan in 1986. The ID3 algorithm is based on Hunt's algorithm and was serially implemented. The ID3 tree is built in two phases: tree building and tree pruning. Data is sorted at each node during the tree building phase to choose the best unique split attribute.
The main ideas behind the ID3 algorithm are:
• Each non-leaf node of a decision tree corresponds to an input attribute and each arc to a possible value of that attribute. A leaf node corresponds to the expected value of the output attribute when the input attributes are described by the path from the root to that leaf node.
• In a "good" decision tree, each non-leaf node must correspond to the input attribute that is the most informative about the attribute among all input attributes not yet considered in the path from root to root. that node. This is because we would like to predict the output attribute using the fewest possible number of questions on average [2].

### 2.1.1 Entropy

Entropy is used to determine how informative a particular input attribute is over the output attribute for a subset of the training data. Entropy is a measure of uncertainty in communication systems.

The classical formula for entropy, whose value is between 0 and 1, is as follows:

![alt text](https://github.com/jorgedejesus110890/Decision-Tree/blob/main/Entropy.jpg?raw=true)


### 2.1.2 Information gain

The information gain is the measure used by the ID3 algorithm to select the most profitable attribute for separation. Also known as mutual information, information gain aims to reduce information uncertainty. In fact, the mutual information of two random variables X and Y measures the dependency relationship between the two variables: the higher the value of the mutual information, the stronger the dependence between X and Y, that is, in our case, the attribute with the highest information gain separates the data set well, which is why it should be chosen. The mathematical expression of this measure has the form:

![alt text](https://github.com/jorgedejesus110890/Decision-Tree/blob/main/Gain.jpg?raw=true)

### Dataset

The database that has a sample 12 dogs.

![alt text](https://github.com/jorgedejesus110890/Decision-Tree/blob/main/Dataset.jpg?raw=true)

Table 1. Simple data set to determine the risk of dogs.


The data presented in Table 1 present the following attributes:

- Number. It is an ordinal attribute represents the number of dogs from 1 to 12.
- Color. It is a nominal attribute with two different observations, which are: Black and Brown.
- Body Shape. It is a nominal attribute with three different observations, which are: Big, Medium and Small.
- Hair Type. It is a nominal attribute with two different observations which are: Poodle and Smooth.
- Characteristic. It is a nominal decision attribute. Determine if the dog is dangerous or not and its observations are: Danger and Safe.

### Results

The decision tree with ID3 would be as follows:

![alt text](https://github.com/jorgedejesus110890/Decision-Tree/blob/main/Decision-Tree.jpg?raw=true)

Figure 1. The decision tree produced based on the ID3 algorithm.

Conclusions

In this work, the ID3 algorithm to build decision trees is presented, its advantages and disadvantages are shown, an exercise is carried out to see how this algorithm works, the results in section 3. Results give evidence that it is possible to build with precision decision trees from the ID3 algorithm. It can be concluded that from a set of data provided by a specialist in a discipline it is possible to have decision trees through the ID3 algorithm since it is a reliable support and help tool for decision making, it is important to highlight that You must have a consistent and reliable data set, since these types of tools depend on the knowledge provided by the information.

