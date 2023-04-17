# IceCube - Neutrinos in Deep Ice

The goal is to predict a neutrino particle’s direction. You will develop a model based on data from the "IceCube" detector, which observes the cosmos from deep within the South Pole ice.

Help scientists better understand exploding stars, gamma-ray bursts, and cataclysmic phenomena involving black holes, neutron stars and the fundamental properties of the neutrino itself.
# Context
One of the most abundant particles in the universe is the neutrino. While similar to an electron, the nearly massless and electrically neutral neutrinos have fundamental properties that make them difficult to detect. Yet, to gather enough information to probe the most violent astrophysical sources, scientists must estimate the direction of neutrino events. If algorithms could be made considerably faster and more accurate, it would allow for more neutrino events to be analyzed, possibly even in real-time and dramatically increase the chance to identify cosmic neutrino sources. Rapid detection could enable networks of telescopes worldwide to search for more transient phenomena.

Researchers have developed multiple approaches over the past ten years to reconstruct neutrino events. However, problems arise as existing solutions are far from perfect. They're either fast but inaccurate or more accurate at the price of huge computational costs.

The IceCube Neutrino Observatory is the first detector of its kind, encompassing a cubic kilometer of ice and designed to search for the nearly massless neutrinos. An international group of scientists is responsible for the scientific research that makes up the IceCube Collaboration.

By making the process faster and more precise, you'll help improve the reconstruction of neutrinos. As a result, we could gain a clearer image of our universe.

# EDA
Analyzed the data of several files. More details can be found here [icecube-neutrinos-in-deep-ice-eda](https://github.com/IAskarov/IceCube/blob/master/icecube-neutrinos-in-deep-ice-eda.ipynb) or[Kaggle](https://www.kaggle.com/code/ilnuraskarov/icecube-neutrinos-in-deep-ice-eda?scriptVersionId=124947435).



# Model
A neural network was defined having in mind this is a regression problem:
 - 5  linear layers
 - RELU as activation function
 - L1Loss as model metric
 - ADAM as optimizer

LGBM machine learning model was attempted, but it perform poorly, especially in computation time. Score from test set was 1.558 and since the model can't use further trees (because it increases computation time directly with the amount of batches trained) this solution was abandoned. 
More details can be found here [icecube-nn](https://github.com/IAskarov/IceCube/blob/master/icecube-nn.ipynb) or [Kaggle](https://www.kaggle.com/code/ilnuraskarov/icecube-nn?scriptVersionId=124952276).
