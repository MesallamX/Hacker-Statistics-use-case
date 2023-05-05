# Data-Camp-Data-Science-track-Hacker-Statistics-use-case
Hacker Statistics is an interesting application that exemplifies how random simulations can be utilized to determine the probability of achieving a specific outcome. The scenario entails a random walk, where a dice is rolled 100 times, and the results dictate whether the player moves forward or backward. The question that arises is, what is the likelihood of reaching a certain level, such as 60 steps high?

To tackle this question, the simulation is performed numerous times, resulting in an array of final steps. This data is then employed to generate a distribution of final steps, enabling the calculation of probabilities.

The process begins by considering the number of tails obtained after ten coin tosses. To obtain the distribution of this walk, a for loop is employed to simulate 100 runs. After each game, the last number of tails, which indicates the number of tails after ten tosses, is added to the final_tails list. The resulting list encompasses numbers ranging from 0 to 10, representing a distribution.

To visualize the distribution, a histogram is utilized. The pyplot library is imported, and the hist function is called, specifying the requirement for 10 bins. The resulting histogram provides an idea of the distribution, but it may not be entirely smooth.

To enhance the accuracy of the distribution, the simulation is repeated 1,000 and then 10,000 times. The resulting histogram starts to converge towards a bell-shaped curve, similar to the theoretical distribution obtained through analytical pen-and-paper calculations.

Upon running the code, it can be observed from the curve that in approximately 2,500 games out of the 10,000 played, the player ends up with five tails. This demonstrates the potency of random simulations in determining probabilities and obtaining accurate distributions.
