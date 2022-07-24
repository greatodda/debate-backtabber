https://tabbycat.readthedocs.io/en/stable/features/draw-generation-bp.html is a classic overview of how modern tabbing softwares like tabby do Draw generation.

Generally the tabbing softwares make use of the standard hungarian algorithm to determine pairings for each round. While it is difficult to take into account things such as clashes in standard backtabbing, using the complete draw table can make it easier to approximate the scores obtained in silent rounds to a good certainty.

My goal with this project is to de-compile and implementation of Hungarian  and determine the scores teams would have gotten for such a draw to be generated. I expect this to take some time but hopefully this will be done before 2022 USUDC.
