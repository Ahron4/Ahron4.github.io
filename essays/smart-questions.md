---
layout: essay
type: essay
title: "Smart Questions Practically Answer Themselves"
# All dates must be YYYY-MM-DD format!
date: 2026-01-29
published: true
labels:
  - Questions
  - Answers
  - StackOverflow
---

<img width="400px" class="rounded float-start pe-4" src="../img/smart-questions/smart-questions.png">

## Think before you do or something like that

You may have heard the saying, either from a friend or your parents, "Think before you speak," where you consider how your words affect others, checking your tone, and thinking of what to say to avoid any misunderstandings. Even though it seems easy enough to understand and learn, it gets kind of difficult when you are in the heat of the moment during a conversation with someone or towards groups of people. I feel like it is an essential skill to acquire, especially if you are working in customer service-related jobs, such as in the food or retail industry. It takes patience to think about what you want to say and asking good questions since it could make it or break your interaction with someone.

## Coding and Learning Smart

Coding and learning new programming languages and theory can be quite confusing, so it is no brainer that asking questions is the way to go. You can tell that people who "RTFM" or "STFW" as Eric Raymond calls it in is essay *How To Ask Questions The Smart Way* show how passionate and curious they are. What I mean is that they often research to see if a similar question hasn't been posted, then, instead of copying and pasting things like code snippets and very little details, they describe the problem and the overall goal they want to achieve. It tells readers like us that they tried to solve the problem to the best of their abilities and are looking for the community for help. Take Stack Overflow, for instance, it is a Q&A website designed for programmers and developers alike to ask questions on code, debugging help, and many more.

In the following example, we examine the components of a decent question. In this case, someone is asking why scanf() in C leaves a newline character in the buffer.

```
Q: I have the following program:

int main(int argc, char *argv[])
{
    int a, b;
    char c1, c2;
    printf("Enter something: ");
    scanf("%d", &a); // line 1
    printf("Enter other something: ");
    scanf("%d", &b); // line 2

    printf("Enter a char: ");
    scanf("%c", &c1); // line 3
    printf("Enter another char: ");
    scanf("%c", &c2); // line 4

    printf("Done"); // line 5

    system("PAUSE");

    return 0;
}

As I read in the C book, the author says that scanf() left a newline character in the buffer, therefore, the program does not stop at line 4 for user to enter the data, rather it stores the new line character in c2 and moves to line 5.

Is that right?

However, does this only happen with char data types? Because I did not see this problem with int data types as in line 1, 2, 3. Is it right?
```
I would say that this is a very decent question since they acknowledge that they read the documentation and are trying to explain the situation to the community. They explain what they know and what they tried, giving the community a better grasp of the situation. This post has gotten 7 answers with a variety of different answers. The person explaining their question gives us context that they have some knowledge of the C programming language, which saves us a lot of time and gets straight to the point of explaining the alternatives to the question. 

## Act first, ask questions later

Here is what I would say is a non-decent question:

```
Q: What is a NullPointerException, and how do I fix it?

What are Null Pointer Exceptions (java.lang.NullPointerException) and what causes them?

What methods/tools can be used to determine the cause so that you stop the exception from causing the program to terminate prematurely?
```

Surprisingly, 12 people answered this question, but it just shows an overall non-smart question since there is documentation on these types of exceptions. All you have to do is search it up on Google, and you will see documentation from Oracle that explains what a NullPointerException is. Granted, I may not know this person's overall programming experience, and perhaps needed more explanation on these exceptions, but they could have at least included a little bit of context before asking the community for help, since this feels like someone asking the community to do their homework for them. I know it sounds harsh but I am just being honest that you will learn way more if you tried it yourself. If you haven't, then what is the point of learning? 
