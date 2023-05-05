# Hacker-Statistics-use-case
Hacker Statistics is a use case that demonstrates how random simulations can be used to calculate the chances of reaching a certain outcome. The scenario involves a random walk, where a dice is thrown 100 times, and the results determine whether the player moves up or down. The question at hand is what is the chance of reaching a certain level, in this case, 60 steps high.

To answer this question, the simulation is repeated thousands of times, resulting in thousands of final steps. This data is then used to create a distribution of final steps, which allows for the calculation of probabilities.

The process begins with the example of the total number of tails after 10 coin tosses. To find the distribution of this walk, a for loop is used to simulate 100 runs. After simulating a single game, the last number of tails, which represents the number of tails after 10 tosses, is appended to the final_tails list. The resulting list contains numbers between 0 and 10, which represent a distribution.

To visualize the distribution, a histogram is used. The pyplot library is imported, and the hist function is called, specifying that 10 bins are required. The resulting histogram gives an idea of the distribution, but is not very smooth.

To improve the accuracy of the distribution, the simulation is repeated 1,000 times, and then 10,000 times. The resulting histogram starts to converge to a bell-shaped curve, which is similar to the theoretical distribution obtained through analytical pen-and-paper calculations.

From the curve, it can be seen that in around 2,500 games out of the 10,000 played, the player ends up with tails 5 times. This demonstrates the power of random simulations in calculating probabilities and obtaining accurate distributions.
