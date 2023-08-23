# Take Home Quiz 1

## Prompt

In the sport of basketball, when a player is "fouled," they have the opportunity to take two "free-throws," where the
player shoots the ball two times and can give his team one point for each basket made

An important statistic in basketball is a player's free-throw success percentage over the basketball season. For
example, if a player has 10 free-throw attempts made 8 baskets, their percentage is 80%.

Interestingly, the percentage is always rounded to the nearest percent (for the ease of the viewing public, which
probably does not know math). For example, if a player has made 7 out of 22 free-throws, then the reported percentage is
32%.

During a game, the announcer says that a player is making 78% of their free throws at the moment that the player is
fouled. The player makes two free-throw attempts and makes the first one but misses the second attempt. After the
statistics are updated, the player is now making 76% of their free-throws.

For this player, what are all possible numbers of free-throws made and attempted so far this season (including the ones
that were just made)? (Hint: There are a finite number of solutions)

## Solution
Click [here](../assets/take-home-quiz-1.pdf) to view the solution.

## Verification
In Kotlin, the solution can be verified by running the following code:

```kotlin
fun calculatePercentages(
    percentInitial: Int,
    percentFinal: Int,
    successes: Int,
    rounds: Int,
    iterations: Int,
): MutableList<Pair<Int, Int>> {

    val solutions = mutableListOf<Pair<Int, Int>>();

    assert(iterations > 1) { "iterations $iterations must be greater than 1" };

    for (n in 1..iterations) {
        for (s in 1..n) {
            val rawPercent = s.toDouble() / n.toDouble();

            val percentRounded = Math.round(rawPercent * 100).toInt();

            val finalSuccesses = s + successes;
            val finalRounds = n + rounds;

            val rawFinalPercent = finalSuccesses.toDouble() / finalRounds.toDouble();
            val finalPercentRounded = Math.round(rawFinalPercent * 100).toInt();

            if (percentRounded == percentInitial && finalPercentRounded == percentFinal) {
                solutions.add(Pair(s, n));
            }

        }
    }

    return solutions;
}

//sampleStart
fun main() {
    val iterations = 1000;

    calculatePercentages(78, 76, 1, 2, iterations).forEach {
        println("s: ${it.first}, n: ${it.second}")
    }
}
//sampleEnd
```

