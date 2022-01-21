---
title: "Git Branch Strategy"
date: 2022-01-17
draft: false
description: "Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency"
tags: ['git', 'version control', 'branching', 'beginners']
blog_list_image: images/git-branch.png
transform: 0%
images: ['images/git-branch.png']
author: Saúl Zalimben
slug: git-branch-strategy
idiom: English
---

In this post, we will go over Git Branching Strategy and Git Workflows, it will not focus on comparing Git Branching Models, nor explain one by one since that story has been told more than once, but you will be able to find the links and examples in this post.

If you're looking for a *Git Tutorial*, I recommend my previous post on it, [Git Explained by DEV Community](blog/english/posts/git-explained).

----

## Introduction

[Git](https://git-scm.com/doc) has become the *de facto* standard for source control management. Branching is an essential feature of a [VCS](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control) (version control system), that allows developers to diverge from the main branch and continue their work on multiple feature branches in parallel, without affecting the main branch. 

>
> Git does NOT enforce any particular branching strategy.
>

Git allows teams to tweak Git Workflows, as it fits the team’s culture. As a result, teams and organizations are often required to choose a particular branching strategy that matches their release cadence, while optimizing productivity depending on their team size, strengths and weaknesses.

Some Git Branching Models are the best in certain situations, but none can be considered the *"best"*, therefore, it is important to mention that there is no such thing as "Best Git Branching Model" or "Best Git Workflow" or "Best Gitflow" or any of its variations, but what you may find is *"A successful Git branching model for X situation"* which is true as Git Workflows are flexible and change as needed, so in certain situations, one Git Workflow is better than others, simple as that.

>
> There is no such thing as *"Best Git Branching Model"*.
>

## Git Workflows
A Git Workflow is a recipe or recommendation for how to use Git to accomplish work in a consistent and productive manner and deal with the branching problem.

> **Gitflow is not Git Workflow**
>
> In some cases, the term Gitfow is used to refer to the actual Git Workflow used by a team or organization, but this is incorrect. A Git Workflow could be any of the Git Branching Strategies that the team or organization is using and a Gitflow is a type of Git Workflow.

### Git Branching Models
Here a list of some well-defined models: 

#### [Git Commonflow](https://commonflow.org/)
![Commonflow](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/uz3yevyu7g6akubo6gna.png)

#### [Gitflow](https://nvie.com/posts/a-successful-git-branching-model/)
![Gitflow](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/v2ojn0uyvx96vuqa65j3.jpg)

#### [GitLab Flow](https://about.gitlab.com/solutions/gitlab-flow/)
![GitLab Flow](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/39585l2n34br7xo3wd8q.jpg)

#### [GitHub Flow](https://docs.github.com/en/get-started/quickstart/github-flow)
![GitHub Flow](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ecy82dtuqv34li88lrd6.png)
 
#### [Trunk Based Development](https://trunkbaseddevelopment.com/)
![Trunk Based Development](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/doaeef4dqbpm729w0vyi.png)

This post performs a [comparative analysis](https://dev.to/arbitrarybytes/comparing-git-branching-strategies-dl4) of the three most popular branching strategies, namely, Git Flow, Trunk Based Development and GitHub Flow.

### Custom Git Branching Models
There are also several custom Git Branching Models; In some cases, teams take a well-defined git workflow and modify it based on the needs of the project. Therefore, it is very common to find mutations of the git branching models mentioned above.

#### Example: [Git Environment Branching Flow](https://dev.to/preethamsathyamurthy/git-branching-and-branching-strategy-4mci)
This strategy focuses on branches per environment (development, staging and production), where each branch is restricted by rules.

Initially, three branches are required: staging, develop and master (or main).

| Branch  | Environment |
|---------|-------------|
| develop | Development |
| staging | Staging     |
| master  | Production  |

![Git Environment Branching Flow](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/w96pg7r5kaeabhboeutz.jpg)

## Conclusion
There is [No Silver Bullet](https://www.researchgate.net/publication/220477127_No_Silver_Bullet_Essence_and_Accidents_of_Software_Engineering) for Git Branching, each strategy has a list of pros and cons. Choosing the "best" requires researching the well-defined models and the needs of the project, and checking if the model covers all you need or maybe a custom model based on a well-defined.

Also, it is okay to make mistakes when selecting the correct model, if that happens remember you can always modify the current strategy or move to another one, Git allows that.

----

If you like this article, don't forget to share it within your network.

## References
- [Git Docs](https://git-scm.com/doc)
- [Version Control System](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)
- [No Silver Bullet](https://www.researchgate.net/publication/220477127_No_Silver_Bullet_Essence_and_Accidents_of_Software_Engineering) 
- [Comparing Git Branching Strategies](https://dev.to/arbitrarybytes/comparing-git-branching-strategies-dl4)
- [Git Branching and Branching Strategy](https://dev.to/preethamsathyamurthy/git-branching-and-branching-strategy-4mci)
- [Introduction to Git Version Control Workflow](https://build5nines.com/introduction-to-git-version-control-workflow/)
- [YAGBW - Yet Another Git Branching Workflow](https://dev.to/andou/yagbw-yet-another-git-branching-workflow-hf4)
