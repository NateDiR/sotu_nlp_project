## Topic Modeling State of the Union Addresses 1970-2022

The goal of this project is to distill the main topics of each State of the Union speech delivered by a president between 1790 and 2022. 

[MVP Script](mvp_script.ipynb)

As a first step, I preprocessed the data using SpaCy, CountVectorized the data with sklearn, did some dimensionality reduction with TruncatedSVD, and pulled out the top 10 topics:

__Topic  0:__
*government, year, congress, united, states, country, state, great, law, people*

__Topic  1:__
*program, year, world, new, work, need, help, america, nation, federal*

__Topic  2:__
*program, dollar, year, fiscal, united, war, expenditure, policy, administration, states*

__Topic  3:__
*man, law, court, service, business, department, dollar, legislation, national, need*

__Topic  4:__
*war, dollar, man, expenditure, power, people, great, peace, public, state*

__Topic  5:__
*nation, administration, state, policy, man, energy, effort, continue, program, power*

__Topic  6:__
*mexico, united, war, states, american, texas, mexican, man, peace, army*

__Topic  7:__
*mexico, country, nof, nthe, texas, mexican, nto, nand, army, public*

__Topic  8:__
*state, constitution, dollar, american, government, program, department, business, canal, united*

__Topic  9:__
*world, government, nof, nthe, american, free, shall, nand, nto, great*


The results were largely meaningless. I need to re-think my approach.

- __Text Preprocessing:__ I should try adding in more custom stop words, and maybe cleaning up the dataset using regex for errors like 'nto' and 'nof'.

- __Vectorization:__ I should try something other than a CountVectorizer for this dataset as there is a lot of noise from those results. Tfid seems like a good option.

- __Dimensionality Reduction:__ I should try additional techniques for dimensionality reduction beyond TruncatedSVD.

- __Results:__ Instead of 10 topics overall I should be producing 3-5 topics on a per-docoument basis so they are more discrete.

A lot of work to be done.