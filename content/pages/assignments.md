---
content_type: page
description: This section provide the homework assignments of the course along with
  links to related online development tools and environments.
draft: false
learning_resource_types:
- Assignments
ocw_type: CourseSection
title: Assignments
uid: 27f22ab8-bfd3-2eae-bc60-f5dbb135c98e
video_files:
  video_thumbnail_file: null
video_metadata:
  youtube_id: null
---
**NOTE**: The homework assignments for this class require access to the following online development tools and environments that **may not be freely available to OCW users**. The assignments are included here as examples of the work MIT students were expected to complete.

{{% resource_link "d1190b20-4086-47e3-97d7-43776be86983" "Message Passing Interface (MPI)" %}}: Standardized and portable message-passing system designed by a group of researchers from academia and industry to function on a wide variety of parallel computers.

{{% resource_link "bf2cec05-0d00-4ef1-a526-6a9fa18aac74" "Star-P:" %}} Technical computing software that offers an open platform architecture that helps to integrate software and hardware from various high performance computing (HPC) sources, and supports popular desktop tools, numerical libraries and hardware accelerators.

{{% resource_link "1289a8c2-85f0-4533-884b-a26baba680fe" "The Julia Programming Language:" %}} A high-level, high-performance dynamic language for technical computing, with syntax that is familiar to users of other technical computing environments. It provides a sophisticated compiler, distributed parallel execution, numerical accuracy, and an extensive mathematical function library.

{{% resource_link "df6f1c86-c5ee-4aa2-869c-51f473e948e7" "Amazon Elastic Compute Cloud (Amazon EC2):" %}} A web service that provides resizable compute capacity in the cloud. It is designed to make web-scale computing easier for developers.

{{% resource_link "0035883c-4790-4406-8b00-9f9cb29a3ff9" "Hadoop MapReduce:" %}} A programming model and software framework for writing applications that rapidly process vast amounts of data in parallel on large clusters of compute nodes.

## Homework 1

In this assignment you will be exposed to different models of parallel computation. The goal is simply to say "hello world" through different tools and environments so you know how to access them.

We will use four combinations of tools and environments: MPI on a cluster, Star-P on a cluster, Julia on Amazon Elastic Compute Cloud (EC2), and Julia on multi-core. There is nothing too special about these combinations; it is also possible to run MPI on EC2 or Julia on a cluster, for example.

The tools and environments you will use are:

1. MPI on a cluster
2. MATLAB® with Star-P
3. Julia on EC2
4. Julia on multi-core

For each section of the assignment, copy a transcript of the interesting parts of your terminal session to a text file

Sample Files: MPI example program in C ({{% resource_link dbf4481f-e6e6-33c3-5c28-1f1b2de0f46d "C" %}}), MPI example program in Fortran ({{% resource_link 129aec8d-d01b-e955-c3e7-360e78e83ced "F" %}})

## Homework 2

In this assignment you will implement a statistical analysis using the MapReduce paradigm with Hadoop, and run your analysis at a reasonable scale on a cluster of Amazon EC2 instances.

The tools and environments you will use are:

1. Running Hadoop clusters
2. Running MapReduce jobs
    1. Using Java
    2. Using other languages

Suggested reading: Sections 3.1 through 3.3 of the book

Lin, Jimmy, and Chris Dyer. *Data-Intensive Text Processing with MapReduce*. Morgan & Claypool, 2010. ISBN: 9781608453429. \[Preview with {{% resource_link "b1b9f559-d949-4260-a883-be303eae06fd" "Google Books" %}}\]

Tasks to perform:

#### Analyzing bigrams

This exercise is adapted from material accompanying Lin and Dyer's book. You are welcome to consult any material you want to help solve this problem. However, if you encounter a full solution to this particular problem on the internet, please do not use it.

Bigrams are sequences of two consecutive words. Understanding which bigrams occur in natural language is useful in a variety of search and textual analysis problems. We will use MapReduce first to count the unique bigrams in an input corpus, and then to compute relative frequencies (how likely you are to observe a word given the preceding word).

**Counting bigrams**

Modify the word count example code to count unique bigrams instead. How many unique bigrams are there? List the top ten most frequent bigrams and their counts.

**Relative frequencies**

Some bigrams may appear frequently simply because one of their words is especially common. We can obtain a more interesting statistic by dividing the number of occurrences of the bigram "A B" by the total number of occurrences of all bigrams starting with "A". This gives *P*(*B*\\*A*), the probability of seeing "B" given that it follows "A".

Pick a word, and show the relative frequencies of words following it. What pairs of words are especially strongly correlated, i.e. *P*(*B*\\*A*) is large?

Section 3.3 of the book discusses a technique for computing this result in a single MapReduce job, using fancy features of the framework. You do not have to use this technique, and may instead use multiple MapReduce jobs if you wish.

**Obtaining input data**

You can use the input data available on the homework page of the class website, or you may select your own corpus of input text. {{% resource_link "abe08639-3895-4876-b4e6-9ee232637217" "Project Gutenberg" %}}, is a good source of interesting texts. There is no particular requirement on the size of data to use, but it should be interestingly large, e.g. the complete novels of Charles Dickens. To make the assignment more fun, entirely at your option, you may wish to compare statistics of different authors, time periods, genres, etc.