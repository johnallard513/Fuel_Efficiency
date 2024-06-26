# Fuel Efficiency Study

For this project, I'm examining the relationship between various vehicle attributes and their effect on fuel efficieny. My research primarily involves investigating engine size, cylinder count, and horsepower of various manufacturers and any trends that appear across model years. Due to the complex relationship between the features, Given the complex relationship between the atributes, I'm using PCA and tSNE techniques to examine the data.

My goals are to group similar vehicles into groups for customer segmentation and advertising purposes for a ficiontal car dealership. 

## Dataset

The dataset I'm using was provided by the MIT Applied Data Science Program and consists of 398 vehicles made between 1970-82 by a wide variety of manufacturers. I originally used this project as my milestone project submission, and now that I've completed the course I've decided to expand it to include in my professional portfolio.

![Carlot](Images/Carlot.jpg)

## Libraries

* Matplotlib
* Seaborn
* Pandas
* Numpy
* Collections
* Mpl_toolkits
* Sklearn

## Questions 

* Do cars with high, mid, or low MPG typically share similar engine characteristics?
* Are there any manufacturers who specifically make vehicles with certain engine characteristics?
* What are the trends by model year?
* What style of vehicles typically have the best MPG?
* Which types of vehicles have the most powerful or least powerful engines?
* Is horsepower more heavily impacted by displacement or cylinder count?
* How does MPG change by model year for specific types of vehicles? (ie. midsized, compact)
* How much variance do we see among the variables?

## Findings
Engine displacement, horsepower, cylinder count, and vehicle weight work together in a complex way to determine the overall MPG. But generally, cars with higher MPG have low weight and high engine displacement. Vehicles made after 1980 also have much better fuel efficiency, as well as smaller engines and less horsepower.

Horsepower's also determined by a complex relationship between engine size and cylinder count. You can see from the 2D chart of cylinder count vs. horsepower that vehicles with more cylinders typically have higher horsepower, but there's overlap between the highest horsepower 4 cylinder engines and the lowest horsepower 8 cylinder engines. And from the 3D graph that includes engine size, you can also tell that this affects horsepower as well, but there are still small engines with high horsepower and large engines with lower horsepower.

There's quite a bit of variance for every variable but the averages typically stay towards the lower mid-range and there doesn't seem to be too much variance between the manufacturers.

![PCA](Images/PCA.jpg)

![TSNE](Images/TSNE.jpg)

## Segmentation

Since there aren't any clear correlations between individual variables, you can't say definitively to segment the vehicles by this or that. Generaly, though, the data suggests you should focus on a balance of engine size and MPG.

Customers who want larger vehicles typically aren't as concerned with MPG, so powerful, low MPG can be grouped together. Larger, more powerful vehicles with higher MPG should have their own group also since some people prioritize both fuel efficiency and power. For small/mid-sized vehicles, high MPG vehicles should be grouped together and high-acceleration vehicles should be grouped together since these are the 2 biggest priorities for customers looking for smaller vehicles.

Within the groups, the dealership should organize the vehicles by model year since there are such strong trends regardless of brand.


