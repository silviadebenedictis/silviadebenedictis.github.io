---
layout: project
type: project
image: img/traffic.png
title: "Traffic Map"
date: 2020
published: true
labels:
  - Python
summary: "I developed a program that creates a map with markers for all the traffic collisions from the input file"
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

Traffic Map is a program that asks the user for the name of a CSV file, name of the output file, and creates a map with markers for all the traffic collisions from the input file. It uses collision data collected and made publicly by a state, such as New York City Open Data. I worded on this individually as part of my CS class assignment. As I was already familiar with Python, I had 


Here is some code that illustrates how we read values from the line sensors:

```cpp
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

You can learn more at the [UH Micromouse News Announcement](https://manoa.hawaii.edu/news/article.php?aId=2857).
