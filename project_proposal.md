#### Statement of Need:

In American politics, the President's State of the Union address has played many roles since its inception in 1790. Traditionally, State of the Union addresses have been used by Presidents to prioritize *'such measures as he shall judge necessary and expedient'* to the Congress. From 1790 until 1913, the address was typically delivered as a written report to the Congress. However after 1913, President Wilson began the regular practice of delivering the State of the Union to a joint session of Congress in person as a means of rallying support for the president's agenda. 

Calvin Coolidge delivered the first State of the Union over the radio in 1923, Harry Truman delivered the first State of the Union on television in 1947, Lyndon B. Johnson delivered the first evening televised address in 1965, and President Reagan began doing so every year in January. 

As time has gone on and mass communications technologies have proliferated, the State of the Union has morphed from a President's written update to Congress, to an annual speech where the President addresses the American people directly-- highlighting the forward-facing goals and backward-facing accomplishments of an administration, as well as signalling to Congress what legislation the President feels shoyld be prioritized in the upcoming year. 

Because State of the Union addresses are watched by so many voters, all manner of lawmakers, interest groups, and advocacy organizations lobby the White House and vie for the briefest of mentions in a SOTU speech. 

In this project, we will analyze State of the Union addresses from George Washington in 1790 to Joe Biden in 2022 using Natural Language Processing. The goal will be to identify the main topics of each address, and explore whether legislative action was subsequently taken on those topics mentioned by a President during his State of the Union.

Our hypothetical audience for this project is executives at any of the above-mentioned organizations who have a business stake in the SOTU. The practical application of this project is determining whether or not it's worth lobbying to have your issue mentioned in an SOTU address.

#### Data Description:
- The Data for this project was sourced from [Kaggle](https://www.kaggle.com/jyronw/us-state-of-the-union-addresses-1790-2019), with the most recent SOTU address by President Biden being added manually.

- In this dataset, an individual obersvation includes President name, year, title (e.g. First/Eighth State of the Union), and the entire text of the State of the Union address delivered in that year, by that President.

#### Tools:
- **scikit-learn**, **gensim**, **SpaCy**, and **NLTK** for text processing.
- **Pandas**, and **NumPy** for data manipulation.
- **Matplotlib**, **Seaborn**, and **Tableau** for visualization.

#### MVP Goal:
* Basic output showing topics for each State of the Union speech.
