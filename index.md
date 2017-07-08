## Welcome to my Github Pages Blog

Simple blog using Jekyll, using the Minimalism theme. [See the Github Repo here.](https://github.com/tz-hmc/tz-hmc.io/edit/master/index.md) Mostly to document the progress made this summer for cybersecurity research for UMich. 

# Blog Posts

**[Working on an Automated Testing Setup.](https://docs.google.com/document/d/1JNf_rxMY7UrNnkQix34awKr_We_I4zh7ElJqcFjU-Kw/pub)**

_Tina Z, June 2, 2016_
 
My project for the first week of summer is to try replicating the results for the Current Events paper, which described being able to recognize what websites were accessed based on frequency analysis of a computer’s power line, using a machine learning SVM. Initially I hoped to use old data sets to train a rudimentary machine learning SVM using the open source library libsvm, but we couldn’t find the hard drive with the right data (or the data in the right hard drive.) Seeing as a few years of PhD research data may now be lost in the void, I decided to collect power traces for each website accessed by a Raspberry Pi, computing a FFT, and formatting data sets to be recognized by the machine learning library. 

**[Picking features and implementing LibSVM.](https://docs.google.com/document/d/12mLWdKFwfdn2WNTxsXAfkJl5bkwkFr72GxnQAuGq1Lk/pub)**

_Tina Z, June 9, 2016_
 
Last week I wrote a few scripts to automate collecting data on a Raspberry Pi, and now that I finished collecting data I can finally implement the machine learning algorithm that was mentioned in the previous week’s blog post. 
 
Without going too much into the details, in machine learning a support vector machine can train itself to classify data, mapping the data sets to the outputs, by first analyzing a training set of data. Then, it can be used to operate on real word examples.

**[Doing a basic link budget for RF transmission.](https://docs.google.com/document/d/1XYmpHfy2XEb6mxDUaHyev_ky2Ju2FJ05tbH8qmTYbEQ/pub)**

_Tina Z, June 23, 2016_
 
To ensure we have the right range and right power to transmit and receive RF, we usually do a RF link budget to make sure it’s feasible. Instead of multiplying gains and such, this is usually done by adding the logs of the gain ratios, which usually makes this process a bit easier.

**[Reading hard drive SMART status and badblocks output.](https://docs.google.com/document/d/1XYmpHfy2XEb6mxDUaHyev_ky2Ju2FJ05tbH8qmTYbEQ/pub)**

_Tina Z, June 23, 2016_

A hard drive under constant acoustic interference won't be able to write to a block, so its firmware may be mislabelling the memory it tried to write as a bad sector on it SMART status. We wanted to check, with smartctl and badblocks, whether this was actually true for 4 different hard drives. (spoiler alert: some discrepancies, nothing confirmed.)

**[Checking how analog voltages on digital input pins are read.](https://docs.google.com/document/d/18ObQTojR0cTgyn9_91cCYQSe1TOHkaWSz7KwzBQqrqI/pub)**

_Tina Z, July 7, 2016_

To make that a future setup would work for some project, this week we wanted to check whether an analog voltage could be interpreted ‘correctly’ by a digital input pin without the microprocessor being damaged or destroyed. This would definitely vary per chip/manufacturer, but we wanted a quick test to see whether peak-to-peak AC voltage, at the voltage interpreted as a digital high, would actually be seen as high. Most MCU spec sheets seem to recommend not giving the input pins less than -0.2V, so we wanted to check whether lower voltages will actually break one. Most GPIO pins have Schottky diodes around them so that negative voltage/too positive voltage would be accounted for. 


### Blog Posts using Markdown

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

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/tz-hmc/tz-hmc.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.
