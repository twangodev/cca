---
hide:
  - toc
---
# AP US Government and Politics Score Calculator

When an AP Exam is administered, psychometric analysis determines the score ranges corresponding with each AP Exam score (5, 4, 3, 2, and 1) based on a composite score scale that combines and weights the exam parts. Due to minor variations in exam difficulty, the number of points corresponding with each AP Exam score can vary on different exams. Because this practice exam was never administered, AP has developed these estimated score ranges that teachers can use to approximate AP Exam scores. We caution that these ranges, and the resulting AP Exam scores, are only estimates, and student performance on this practice exam does not necessarily predict performance on a different exam.

#### AP Score Conversion Chart
| Composite Score Range | AP Exam Score |
|-----------------------|---------------|
| 99-120                | 5             |
| 91-98                 | 4             |
| 73-90                 | 3             |    
| 53-72                 | 2             |
| 0-52                  | 1             |

!!! note
    Use this calculator to estimate your AP US Government and Politics score.

Calculate your score by entering the number of correct multiple-choice questions and free-response questions in the code below, then run the code to see your score.

```kotlin
import kotlin.math.round

fun main() {
    //sampleStart
    val mcqCorrect = 0 // Out of 55
    val frqQ1 = 0 // Out of 3
    val frqQ2 = 0 // Out of 4
    val frqQ3 = 0 // Out of 4
    val frqQ4 = 0 // Out of 6
    //sampleEnd

    val weightedSection1Score = mcqCorrect * 1.0909
    val frqQ1Weighted = frqQ1 * 5.0
    val frqQ2Weighted = frqQ2 * 3.75
    val frqQ3Weighted = frqQ3 * 3.75
    val frqQ4Weighted = frqQ4 * 2.5

    val weightedSection2Score = frqQ1Weighted + frqQ2Weighted + frqQ3Weighted + frqQ4Weighted

    val compositeScore = round(weightedSection1Score + weightedSection2Score)

    val score = when {
        compositeScore >= 99 -> 5
        compositeScore >= 91 -> 4
        compositeScore >= 73 -> 3
        compositeScore >= 53 -> 2
        compositeScore >= 0 -> 1
        else -> 0
    }

    println("Your score is: $score")
    println("Your composite score is: $compositeScore")

}
```