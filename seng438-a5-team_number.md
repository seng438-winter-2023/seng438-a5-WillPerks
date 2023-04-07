**SENG 438- Software Testing, Reliability, and Quality**

**Lab. Report \#5 – Software Reliability Assessment**

| Group \#:       |   |
|-----------------|---|
| Student Names:  |   |
|                 |   |
|                 |   |
|                 |   |

# Introduction

The purpose of this lab was to learn how to conduct analysis of integration test data using reliability assessment tools. The tools used included C-SFRAT which is an open source software developed by python for reliability growth testing, and Reliability Demonstration Chart (RDC). Using both of these methods was able to help increase our understanding in regards to reliability testing and failure data and how they play a role in software testing as a whole.


# Assessment Using Reliability Growth Testing 

How we went about selecting the two top models is by plotting all of them using the C-SFRAT tool and going to the Model Comparison section and then sorting the graphs by their Critic (Mean) values, we did not include the graph labeled GM (None).  From this we picked the two graphs that had the greatest values.

After choosing the two graphs to look at in more detail, we have to decide what part of the data is viable for further analysis.  For both of the graphs the interval from 1 to 12 is acceptable.  However, from interval 12 to 16 the data is not viable.  This is because the data deviates from the original data by a significant amount.

MVF Graph:

<img src="Img_A4/R_OLD.png" alt="Img_A4/R_OLD.png" width="360"/>

Intensity Graph:

<img src="Img_A4/R_OLD.png" alt="Img_A4/R_OLD.png" width="360"/>

If we are given a target failure rate we can look at the graphs that we have created and decide whether the program meets the target.  Unfortunately, we don’t know the exact value of the failure rate/MTTF of the program which makes it difficult to do an accurate comparison to the target failure rate. 

One advantage for using reliability growth analysis is it is easy to determine whether or not the program/application meets a target failure rate.  One drawback of this is that when producing the graphs it is a lot to take in all at once, for example sometimes there can be upwards of 25 graphs produced.


# Assessment Using Reliability Demonstration Chart 

Normal:

<img src="Img_A4/R_OLD.png" alt="Img_A4/R_OLD.png" width="360"/>

Half:

<img src="Img_A4/R_OLD.png" alt="Img_A4/R_OLD.png" width="360"/>

Double:

<img src="Img_A4/R_OLD.png" alt="Img_A4/R_OLD.png" width="360"/>

How we decided on 42 as the MTTF is by trial and error.  We started with 50 and found out that it was too big, so we decreased the value until the graph was below the line that marks the red and yellow area (the Reject and Continue areas).

We found that while using the RDC software, it created a nice visual graph of the data plotted which made it easy for us to interpret the graph.  We could make changes to the graph and immediately see the impact it had.  One downside to this is that for getting the MTTF value it was not 100% accurate because how we calculated it is by guessing a value and seeing how close it was.  We would repeat this process until the graph got very close to the Reject area.  Although we tried to make it as close as we could by looking at the graph, it is still an inaccurate way of calculating the MTTF due to human failure.


# Comparison of Results

Both Reliability Growth Test (RGT) and Reliability Demonstration Chart (RDC) let you perform analyses on the failure rate/MTTF of a program.  RGT does not give you an exact or even rough value for what the MTTF is, however it produces lots of graphs which can be interpreted in different ways assuming you have an in depth understanding of the RGT software.  RDC on the other hand, does not give you nearly as many graphs to interpret but gives you a rough value for the MTTF.  Also, it allows you to change the target MTTF which in turn changes the graph.

# Discussion on Similarity and Differences of the Two Techniques

In terms of the similarities of the two techniques, both methods required the input of the same failure dataset. Furthermore, both techniques are involved in determining the reliability of a system through analysis of data. Both use some sort of failure time such as MTTF or other failure rate.

When it comes to differences, reliability growth testing is able to utilize not only the inter failure time but also the failure count. The Reliability Demonstration Chart technique however is able to only use the inter failure time. RDC is also used for products/systems that have been designed while reliability growth testing can be used for increasing the reliability of a product while in its developmental phase.


# How the team work/effort was divided and managed

When it came to dividing the work and effort, everyone made sure to install and have the tools required for the lab up and running. Two of the members worked together on the first part while the other two members worked on the second part. The report and analysis was then done together by the group as a whole.

# Difficulties encountered, challenges overcome, and lessons learned

In the beginning it was a bit difficult to understand which software worked with our machines as 3 out of 4 members have MacBooks. Once everything was installed, the rest of the lab was relatively easy. We were able to learn about how failure data could be analyzed and utilized to the advantage of the software testers.

# Comments/feedback on the lab itself

In terms of the lab itself, the initial setup was something that we struggled with. For the instructions, it could have been helpful if a bit more information on how to interact with the software needed for this lab such as C-SFRAT was provided. The lab was informative in terms of giving us the knowledge on how to work with failure data testing. Overall, it took a bit of time initially but was a smoother process as the lab progressed.
