# What makes a good ramen? Feature extractions and overall EDA 
<img src="https://glouton.b-cdn.net/u/recipes/thumbs/14252.jpg" width="1280" height="650">



<!-- Add banner here -->

The aim of this project is to observe and analyse a dataset of ramen ratings. The dataset has been taken from https://www.kaggle.com/datasets/residentmario/ramen-ratings.

<!-- Add buttons here -->

<!-- Describe your project in brief -->

<!-- Some badges that you could use -->

<!-- Add a demo for your project -->

<!-- After you have written about your project, it is a good idea to have a demo/preview(**video/gif/screenshots** are good options) of your project so that people can know what to expect in your project. You could also add the demo in the previous section with the product description.

Here is a random GIF as a placeholder.

![Random GIF](https://media.giphy.com/media/ZVik7pBtu9dNS/giphy.gif) -->





# Table of contents

<!-- After you have introduced your project, it is a good idea to add a **Table of contents** or **TOC** as **cool** people say it. This would make it easier for people to navigate through your README and find exactly what they are looking for.

Here is a sample TOC(*wow! such cool!*) that is actually the TOC for this README. -->

- [Table of contents](#table-of-contents)
- [Dataset contents](#dataset-contents)
- [Questions](#questions)
- [Demo Preview](#demo-preview)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Issues](#issues)

## Dataset contents

This dataset originally come from The Ramen Rater, a product review website dedicated to ramen only.
The dataset contains 2580 rows that correspond to 2580 product reviews.
In other words, one row means one single ramen product review.
The higher the number, the more recently the ramen product is reviewed.
The table has 7 columns:
- Brand
- Variety(label, the product name)
- Country
- Style (is it in pack? in cup? in bar?)
- Ratings ( Stars refer to the ramen quality  on a 5-point scale)

## Questions
Three questions have been raised, from the easiest question to answer to the hardest one.
1) How is ramen manufacturing internationally distributed?
2) Is there a relation between the ratings and the product's style?
3) At last but not least, What makes a good ramen?


## Demo Preview

<img width="608" alt="Capture d’écran 2022-07-07 à 01 25 30" src="https://user-images.githubusercontent.com/82478538/177659473-de19db27-20fd-4817-b2c7-83d80902759d.png"> <img width="584" alt="Capture d’écran 2022-07-07 à 01 26 18" src="https://user-images.githubusercontent.com/82478538/177659520-30a6050b-3775-4772-ab42-bc445075322d.png"> <img width="563" alt="Capture d’écran 2022-07-07 à 01 26 58" src="https://user-images.githubusercontent.com/82478538/177659528-1a0533b2-c231-4d8a-a446-659adb8f05f9.png"> <img width="522" alt="Capture d’écran 2022-07-07 à 01 27 22" src="https://user-images.githubusercontent.com/82478538/177659532-b10aeb3d-d53f-4cc1-83c2-39199448feca.png">


## Installation

Here are the command lines of the production environment.

```sh
import pandas as pd
import seaborn as sn
import matplotlib.pyplot as plt
import fuzzywuzzy
from fuzzywuzzy import process
%matplotlib inline
from fuzzywuzzy import fuzz
```


## Usage

- It could be interesting to compare the ramen ratings with other product (such as pasta, wine, chocolate...) reviews.
- A 'ramen' dataset with the price of each product coul explain that the purchases of ramen did not get the highest rating but the highest distribution.


## Results

Here are some results from the data analysis in order of the questions.

- Most ramen products are produced by Japan, the USA and South Korea.
- More than 59% of noodle are sold in pack but the style that is the highest rated is the bar.
- Pack noodles has the most distributed noodle style ==>  sellers mostly buy noodle in pack.
- Chicken and beef ramen are the highest distribution. It means that most people buy chicken or beef ramen.
- At most styles pork and beef are usually rated higher compared to chicken and shrimp.
- Noodles and ramen are the most consumed types of 'ramen'.
- No spicy noodles are the most distributed and they get the highest rating.

## Issues
[(Back to top)](#table-of-contents)

- Missing values
- A lot of 'unspecified' values when features have been extracted
- Handle with categorical values written twice differently
