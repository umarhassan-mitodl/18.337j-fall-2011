---
content_type: page
description: This section provides information on the course project and samples of
  student work.
learning_resource_types:
- Projects
ocw_type: CourseSection
title: Projects
uid: c0426d62-bad7-f3e2-33eb-38753796ea60
video_files:
  video_thumbnail_file: null
video_metadata:
  youtube_id: null
---

{{% resource_link c0426d62-bad7-f3e2-33eb-38753796ea60 "Kinds of Projects" "#1" %}}

{{% resource_link c0426d62-bad7-f3e2-33eb-38753796ea60 "Julia-related Project Ideas" "#2" %}}

{{% resource_link c0426d62-bad7-f3e2-33eb-38753796ea60 "Modern Parallel Linear Algebra Project Ideas" "#3" %}}

{{% resource_link c0426d62-bad7-f3e2-33eb-38753796ea60 "Parallel Algorithms, Libraries Project Ideas" "#4" %}}

{{% resource_link c0426d62-bad7-f3e2-33eb-38753796ea60 "Abstractions and Infrastructure Project Ideas" "#5" %}}

{{% resource_link c0426d62-bad7-f3e2-33eb-38753796ea60 "Tools" "#6" %}}

{{% resource_link c0426d62-bad7-f3e2-33eb-38753796ea60 "Sample Student Projects" "#7" %}}

{{< anchor "1" >}}{{< /anchor >}}Kinds of Projects
--------------------------------------------------

*   problem X on parallel architecture/environment Y
*   parallel algorithm for X
*   performance comparisons
    *   what is best algorithm in environment X?
    *   or in input data case X?
    *   how good is, e.g. MPI message latency and could it be better?
*   debugging and monitoring parallel programs
*   parallel abstractions, platforms (e.g. MapReduce)
*   resource sharing infrastructure
*   cloud infrastructure
*   making technical computing more fun

{{< anchor "2" >}}{{< /anchor >}}Julia-related Project Ideas
------------------------------------------------------------

*   Can use as an implementation language
    *   many parallel algorithms are likely to be much easier in Julia than MPI
*   Or work on the platform itself
    *   whole parallel computing system written in Julia, quite compact
    *   parallel computing base: 1600 lines (multi.j)
    *   distributed arrays: 762 lines

{{< anchor "3" >}}{{< /anchor >}}Modern Parallel Linear Algebra Project Ideas
-----------------------------------------------------------------------------

*   LU without block-cyclic
*   LU with dynamic # of CPUs
*   new SVD algorithm

{{< anchor "4" >}}{{< /anchor >}}Parallel Algorithms, Libraries Project Ideas
-----------------------------------------------------------------------------

*   optimization
*   numerical integration
*   multigrid
*   parallel data structures other than arrays
    *   graphs, tables, sparse arrays

{{< anchor "5" >}}{{< /anchor >}}Abstractions and Infrastructure Project Ideas
------------------------------------------------------------------------------

*   a MapReduce or dataflow framework in Julia
*   some other highly-reusable parallel computation
*   high-level EC2 interface
*   storage
    *   persistent distributed arrays
    *   integrate a distributed FS (HDFS, scidb, sector)
*   cluster sharing tools

{{< anchor "6" >}}{{< /anchor >}}Tools
--------------------------------------

*   What would make technical computing more fun?
*   Watching/choreographing parallel computations
*   Social coding features
    *   collaboration
    *   shared "wisdom"
*   Visualization

{{< anchor "7" >}}{{< /anchor >}}Sample Student Final Projects
--------------------------------------------------------------

Three of the students in the class have provided their final projects for publication on OCW and they are presented here with their permission.

Parallel FFT in Julia: {{% resource_link 2f2063e2-65e9-3930-9f5b-2f6b5d4b94d4 "Slide (PDF - 1.6MB)" %}}, {{% resource_link "7574964c-53fe-ac5d-8956-8be3d0644fdc" "Code (TXT)" %}}, {{% resource_link ba7ef71d-c0fe-a405-860b-7ebf878a5399 "Report (PDF)" %}} (Courtesy of anonymous MIT student. Used with permission.)

Social coding: {{% resource_link "4ab4fd18-15c2-ada2-b213-3ad6ebe0bd47" "Slides (PDF)" %}}, {{% resource_link 699a697c-03e7-4136-53ba-6e8b5c4b87ab "Report (PDF)" %}} (Courtesy of anonymous MIT student. Used with permission.)

Replica-Exchange Molecular Dynamics on Hadoop: {{% resource_link 6f344774-4fb5-97fd-274b-70ecc430f956 "Report (PDF)" %}} (Courtesy of Zachary Ulissi. Used with permission.)