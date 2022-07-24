https://tabbycat.readthedocs.io/en/stable/features/draw-generation-bp.html is a classic overview of how modern tabbing softwares like tabby do Draw generation.

Generally the tabbing softwares make use of the standard hungarian algorithm to determine pairings for each round. While it is difficult to take into account things such as clashes in standard backtabbing, using the complete draw table can make it easier to approximate the scores obtained in silent rounds to a good certainty.

My goal with this project is to de-compile an implementation of Hungarian shuffling and determine the scores teams would have gotten for such a draw to be generated. I expect this to take some time but hopefully this will be done before 2022 USUDC.

One of the key obstacles to accurate backtabbing is the Renyi Entropy cost function but I think that in sizable tournaments with enough number of rooms, the result could be approximated relatively with ease by assigning certain value to each possible draw that could be generated from the given scores and looking at their deviation value from the value assigned to the draw of a silent round. We could thus convert this into a minimization problem. This is similar to how softwares like stockfish bypass excessive calculation. 
