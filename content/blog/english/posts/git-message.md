---
title: "Write Git Commit Messages"
date: 2022-02-10
draft: false
description: "A well-crafted Git commit message is the best way to communicate context about changes to other developers working on that project, and indeed, to your future self."
tags: ['git', 'tutorial', 'beginners']
images: ['images/git-message.png']
transform: 0%
blog_list_image: images/git-message.png
author: Saúl Zalimben
slug: write-git-commit-message
idiom: English
---

This article assumes you already understand basic Git Workflow. If not, I suggest reading previous articles on this series.

---

## Why should you write good commit messages?

> *"When a programmer first creates his code, only he and God know how it works, a few months down the line and only God knows."*

Not sure who said this phrase, but it is so accurate. The same thing happens when we write **Commit Messages**. 

We're often pressed for time when it comes to Git commits, and so we write something random or without meaning in our commit message like "Fixes" or "WIP", even memes, memes!

I challenge you to figure out the following commit message:

` Minor fixes `

Perhaps the most common commit message, but what does it mean exactly? We can ask ourselves so many questions about it.

- Minor fixes on what? 
- What were the fixes? 
- Why fixes were needed?
- ... and many more.

Writing commit messages that are not telling the whole story is a bad practice. Commit messages should be helpful and make sense so people working on the project understand the changes from the message itself.

Using the right commit message helps make it more meaningful and it provides clarity on your updated piece of code, for everyone.

It seems like writing good commit messages is easy and everyone understands the benefits of doing it. Yet, you can find messages like the above.
 
Commit messages can communicate why a change was made, they help the narrative of the project. Poetically, commit messages are telling the story of the project, and you can read it using the `git log` command.

> Don't destroy a good story, build one.
 
## How to write good commit messages?

There are several conventions used by different teams, projects, and developers. I'll just give you some general guidelines and pointers, but it's up to you to decide which convention you want to follow.

> If you work for a company or contribute to open source, you have to adapt to their convention.

Check out [this thread](https://hashnode.com/post/which-commit-message-convention-do-you-use-at-work-ck3e4jbdd00zyo4s1h7mc7e0g) for some commit message conventions, discussion proposed by [@bolajiayodeji](https://hashnode.com/@bolajiayodeji).

### 6 General Rules
- **Capitalization and Punctuation**: Capitalize the first word and do not end in punctuation. 
- **Mood**: Use the imperative mood in the subject line. Example: Add fix for dark mode toggle state. 
- **Type of Commit**: Specify the type of commit. It is recommended and can be even more beneficial to have a consistent set of words to describe your changes. Example: Bugfix, Update, Refactor, Bump, and so on.
- **Length**: The first line should be no longer than 50 characters, and the body should be restricted to 72 characters.
- **Content**: Be direct, try to cut filler words and phrases in these sentences. Examples: though, maybe, I think, kind of.
- **Issue Tracker**:  If you use an issue tracker, add a reference(s). 

### Journalism Questions
When a journalist is writing an article they look to answer who, what, where, when, why, and how. It is similar when we are writing commit messages, we need to answer some questions about the changes. 

Sometimes it is not easy to put in words the changes that we made. To simplify that process and come up with thoughtful commits, consider the following "journalism" questions:

- Why are the changes necessary?
- How do changes address the issue?
- Why have I made these changes?
- What effect have my changes made?
- What side effects do the changes have?
- What are the changes in reference to?

Answering these questions will help you to write a better commit message.

### Commit Message Template 
I merged the *6 General Rules* with *Journalism Questions*, to have a well-format compact template:

![Git Commit Message Template](images/git-message.png)

Where:

- **issue|type:** If you are using an issue tracker, set the reference(s), otherwise, set the commit type.
- **title:** Issue name or a short summary of changes.
- **description:** More detailed explanatory text, if necessary. It should answer the template's questions.

The result is:

![Git Commit Message Template](images/git-message-result.png)


#### Git Configuration
Templates can be added to your **[Git Configuration](https://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration)**, so every time you make a commit:

`$ git commit`

the commit message editor will display the template, and you only have to update it. To tell Git to use the template file (globally), you can use the following command:


`$ git config --global commit.template git-message-template.txt` 


By default, Git uses whatever you’ve set as your default text editor to create and edit your commit and tag messages. To change that default to something else, you can use the `core.editor` setting:


`$ git config --global core.editor vim`


## Conclusion

The most important part of a commit message is that it should be clear and meaningful. It helps you communicate and collaborate with your team. 

There is an existing set of agreed-upon standards you can follow. But, you can tweak the convention to get a more appropriate convention for your team or project.

---
Thanks for reading! Let me know what you think in the comment section, don't forget to leave a ❤️ and share it within your network!

Connect with me on Twitter [@sZalimben](https://twitter.com/sZalimben), and if you like my content you can *[Buy Me a Coffe](https://www.buymeacoffee.com/szalimben)*.

## Resources
- [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
- [How to Write Better Git Commit Messages – A Step-By-Step Guide](https://www.freecodecamp.org/news/how-to-write-better-git-commit-messages/)
- [How to Write Good Commit Messages with Commitlint](https://www.freecodecamp.org/news/how-to-use-commitlint-to-write-good-commit-messages/)
- [How to Write Good Commit Messages: A Practical Git Guide](https://www.freecodecamp.org/news/writing-good-commit-messages-a-practical-guide/ )
- [Customizing Git - Git Configuration](https://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration)