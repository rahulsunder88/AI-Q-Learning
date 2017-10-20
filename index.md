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



### Markdown

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
