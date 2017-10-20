### Markdown
# Artificial Intelligence – Q Learning



## What is Q-Learning?

Q-Learning is a part of Artificial Intelligence, used to determine the state action values for each possible state and its action. Q-Learning starts with all the values as zeroes in the Environment. The Reward for each state action pair helps in determining the Q value for a state action. The agent uses these Q values to traverse to the Goal.

Goal here means the State action pair having the maximum value. It can be any value. We will have it as 100.

Q-Learning is applied to a STATIC environment where we know the total number of States and the possible actions, without this knowledge the agent will not be able to determine the correct path.

I shall try to cover the important topics related to Q-Learning. I will not get into much mathematics to make things simpler. Out of curiosity I have gathered information from various sources and consolidated them here.

A complete iteration in an environment is called an EPISODE.

Let us consider an example for easy understanding:

R - Reward matrix having state in Rows and Action in Columns.
Q - Q matrix having state in Rows and Action in Columns.

Let us take an environment of 5 States and 5 Action:



```markdown






State	Action
		1	2	3	4	5
	1	0	0	-1	0	-1
	2	0	0	0	-1	100
	3	-1	0	0	-0.5	100
	4	0	-1	-0.5	0	-1
	5	0	0	-1	0	100
 


R =





Here are 4 junctions, the agent wants to go the Ice cream parlour from various junctions, the junction 5 is the ice cream parlour, there is a signal between 4 and 3 which takes a long time. They are bidirectional roads connecting each other, if there is no connectivity we give a reward of -1, for the signal we give reward of -0.5, and the road leading to Ice cream parlour is given a reward of 100.




Similarly we have a Q table as follows:



State	Action
		1	2	3	4	5
	1	0	0	0	0	0
	2	0	0	0	0	0
	3	0	0	0	0	0
	4	0	0	0	0	0
Q =




The above Q table is initialized with 0 , we will use the formula given below to calculate the value of the Q(state,action) using the below formula:

Q(state, action) = R(state, action) + Gamma * Max[Q(next state, all actions)]


Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](/Users/rahulchellappa/Desktop/article)
```

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](/Users/rahulchellappa/Desktop/article)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/rahulsunder88/Artificial-Intelligence---Q-Learning/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
