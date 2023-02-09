Project Name: Self Driving Car and Ethics

Project Members: Aser Atawya and Michele Tang

The problem we are trying to work on is developing a self simulation of a self driving car that can accurately and safely navigate roads.

This problem is difficult because it requires a lot of edge cases and generally speaking, many roads have different conditions and physical features, so it is challenging to be comprehensive and reactive like a human is. Even major companies, such as Google and Uber, who have attempted to develop self-driving cars, have struggled to address all of these edge cases. For example, Waymo cars, developed by Google, did not pull over for police (https://slate.com/technology/2022/12/san-francisco-waymo-cruise-self-driving-cars-robotaxis.html).

We want to address these challenges first by narrowing the scope of our project by finding a simulator and trying to successfully train our car on one "type" of that simulator, ex. Driving in daylight on an American local road or driving at night on an American highway.

Some challenges we might have to overcome include, developing thorough training data, considering a diverse range of edge cases, learning more about computer vision, etc.

We are still figuring out exactly what parameters we want to use and what the precise scope of the project is, but generally speaking, success will be defined as minimizing accidents/deaths/damages done by our car in the environment we train it on.

The ethical analysis of self-driving cars needs to address both high-level philosophical principles, such as the definition of fairness and accountability as well as dilemmas particular to the case of autonomous vehicles.

For instance, one of our questions is "should self-driving vehicles be programmed to prioritize your own life at all costs, or should it prioritize saving the most lives in all situations?"

We can't provide a conclusive answer to this question unless we delve deeper into the trolley problem (and other problems) and analyze the implications of our decisions not only from philosophical and ethical perspectives but also from technical and economical perspectives.

To find an answer to this question, we can employ open-source tools such as MIT Moral Machine to identify various scenarios where trade-offs need to be taken.

**Ethical Sweep**

**General Questions:**

- Should we even be doing this?
  - Firstly, we are NOT building a real car that will be on the roads. We are just simulating these vehicles to determine how we can improve their accuracy and safety and to learn more about the process of training them. Additionally, these cars already exist, which makes it very important to do ethics research about how decisions are being made.
- What might be the accuracy of a simple non-ML alternative?
  - The current non-ML alternative of this would just be human drivers, which are unfortunately pretty inaccurate at times and cause accidents all the time.
  - We can't think of a non-ML alternative to do this car simulation and learning process.
- What processes will we use to handle appeals/mistakes?
  - Since we are just simulating driving, there are no "appeals" in the sense that a mistake can be detrimental and irreversible.
  - As for mistakes, since we are not putting this car onto the road, mistakes will be used to improve the car in future iterations. We will document mistakes and retrain the car as needed to minimize future mistakes (especially of similar kinds)
- How diverse is our team?
  - One of the main issues with diversity in car training data is the physical territory of roads and land. Both teammates are capable of driving. Aser and Michele are both most familiar with well paved roads. Aser has only driven in urban areas. Michele has driven in all kinds of areas. We say this just to acknowledge that our understanding of various kinds of roads and environments is limited. Thus, we do want to limit our scope to an environment that we are more familiar with because we can come up with more edge cases. We do not claim that accurate driving in this environment will result in accurate driving in all environments.
  - Additionally, Aser has driven in the US and Egypt and Michele has driven only in the US. We are largely unfamiliar with other countries' driving laws.

**Data Questions:**

- Is our data valid for its intended use?
  - Our data is valid for the development of self-driving cars that can pass the testing cases of a simulator and is resourced from simulations designed specifically for this purpose.
- What bias could be in our data? (All data contains bias.)
  - Our data could only be focusing on specific kinds of environments, most likely well paved roads in an area that has public investment into road infrastructure
  - There could be bias in the kinds of people and objects that the data portrays. For example, the data might only present white pedestrians, which we would have to address. It could also only show trees/plants during one season of the year, which would mean they could look significantly different later on in the year.
- How could we minimize bias in our data and model?
  - We want to limit the scope of the environment so we are not trying to do too much. Then, within that limited scope, we will analyze our training data and determine whether there are cases that are missing (ex. The situations above about skin color, plants, etc.)
  - It is quite essential to break down our analysis to the sub-group level to catch and control any bias. For instance, the rate of pedestrian hit may vary across different races or genders due to imbalance in training data. Even though usually data is the main source of bias, other sources can magnify the existing bias, such as the inductive bias embedded within the machine learning models we are using.
- How should we "audit" our code and data?
  - We can look through a significant portion of our training data to determine whether there is a diverse array of environments
  - We will write down various cases and edge cases and examine our simulator to determine if it is properly addressing those
  - We will look through the various ethics articles we are reading and determine if they are given various perspectives, ex. Is it only based on Western philosophy?

**Impact Questions:**

- Do we expect different error rates for different sub-groups in the data?
  - All datasets are biased in some sort, and this bias is often implicit, so even though we wouldn't incorporate any intrinsic human features, we expect them to be present in the data in some sort. For instance, if we design our machine learning model to work with self-driving cars in left-hand traffic countries, those models will not perform as well in right-hand traffic countries.
- What are likely misinterpretations of the results and what can be done to prevent those misinterpretations?
  - One misinterpretation that could arise is that our car will work for different environments. We will be very specific in our project that it will only be trained on a limited environment
  - Another possible misinterpretation of our ethics results is that there is one correct answer to some of these ethical problems. We will offer different points of views and angles of analysis to address this.
- How might we impinge individuals' privacy and/or anonymity?
  - The development of self-driving cars in reality requires the processing of the driving data of millions of drivers and is continuously fed with new data, often without the consent of drivers. Furthermore, the cameras and the sensors used in self-driving cars record images of streets, pedestrians, cars, and private properties; such data certainly impinge individuals' privacy and anonymity if stored without consent.
