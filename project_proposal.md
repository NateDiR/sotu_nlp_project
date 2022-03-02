#### Statement of Need:

In American politics, the President's State of the Union Address has played many roles since its inception in 1790. 

Traditionally, State of the Union Addresses were used by Presidents to prioritize *'such measures as he shall judge necessary and expedient'* to the Congress. 

From 1790 until 1913, the address was typically delivered as a written report to the Congress. However after 1913, President Wilson began the regular practice of delivering the State of the Union to a joint session of Congress in person as a means of rallying support for the president's agenda. 

Calvin Coolidge delivered the first State of the Union over the radio in 1923, Harry Truman delivered the first State of the Union on television in 1947, Lyndon B. Johnson delivered the first evening televised address in 1965, and President Reagan began doing so every year in January. 

As time has gone on and mass communications technologies have proliferated, the State of the Union has morphed from a President's written update to Congress, to an annual televised speech where the President addresses the American people directly-- highlighting the accomplishments of the previous year of an administration, as well as signalling to Congress what legislation the administration will be prioritizing in the upcoming year. 

Because State of the Union addresses are watched by so many voters, all manner of lawmakers, interest groups, and advocacy organizations lobby the White House and vie for the briefest of mentions in an address. 

In this project, we will analyze State of the Union addresses from George Washington in 1790 to Joe Biden in 2022 using Natural Language Processing. The goal will be to generate insights and trends about the main topics of State of the Union Addresses, and explore how a topic being mentioned by a President during his State of the Union Address affected its legislative propsects in the following year (i.e. How often did Congress pass legislation on an issue the president highlighted in the SOTU?)

Our hypothetical audience for this project is executives at any of the above-mentioned organizations who have a operational stake in the SOTU. Think of the Chamber of Commerce, Planned Parenthood USA, Teamsters Union, PhRMA, UMWA. The practical application of this project is identify broad trends SOTU Addresses cover over time, or whether specific Presidents prefer specific themes. More specifically, We will seek to determine whether or not it's worth lobbying to have your issue mentioned in an SOTU address, by identifying the rate at which issues that were mentioned in a SOTU Address had legislation passed in the subsequent year.

#### Data Description:
- The Data for this project was sourced from [Kaggle](https://www.kaggle.com/jyronw/us-state-of-the-union-addresses-1790-2019), with the most recent SOTU address by President Biden being added manually.

- In this dataset, an individual obersvation includes President name, year, title (e.g. First/Eighth State of the Union), and the entire text of the State of the Union address delivered in that year, by that President.

- Additional features, such as party, age, home state, etc. can be added manually.

#### Tools:
- **scikit-learn**, **gensim**, **SpaCy**, and **NLTK** for text processing.
- **Pandas**, and **NumPy** for data manipulation.
- **Matplotlib**, **Seaborn**, and **Tableau** for visualization.

#### MVP Goal:
* Basic output showing main topics for each State of the Union speech.
