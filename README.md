# Multilingual-Detection-of-Persuasion-Techniques-in-Memes

### **NOTE**: This project was developed for SemEval 2024 - Task 4, which can been explored further [here](https://propaganda.math.unipd.it/semeval2024task4/)

Memes are one of the most popular type of content used in an online disinformation campaign. They are mostly effective on social media platforms, since there they can easily reach a large number of users. Memes in a disinformation campaign achieve their goal of influencing the users through a number of rhetorical and `psychological techniques`, such as `causal oversimplification, name calling, smear`.

The goal of the shared task is to build models for identifying such techniques in the textual content of a meme only (one subtask) and in a multimodal setting in which both the textual and the visual content are to be analysed together (two subtasks).

## TECHNICAL DESCRIPTION

**Subtask 1** - Given only the “textual content” of a meme, identify which of the `20 persuasion techniques`, organized in a hierarchy, it uses. If the ancestor node of a technique is selected, only a partial reward is given. This is a `hierarchical multilabel classification` problem.

**Subtask 2a** - Given a meme, identify which of the `22 persuasion techniques`, organized in a hierarchy, are used both in the textual and in the visual content of the meme `(multimodal task)`. If the ancestor node of a technique is selected, only partial reward will be given. This is a `hierarchical multilabel classification` problem.

**Subtask 2b** - Given a meme (both the textual and the visual content), identify whether it contains a persuasion technique (at least one of the 22 techniques we considered in this task), or no technique. This is a `binary classification` problem. Note that this is a simplified version of subtask 2a in which the hierarchy is cut at the first two children of the root node.
