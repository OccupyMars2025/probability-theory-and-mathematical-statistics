To prove the formula for the number of unordered samples of size \( k \) with replacement from \( n \) elements, we need to demonstrate that the number of such samples is given by:

\[ \binom{n+k-1}{k} \]

### Proof:

1. **Understanding the Problem:**
   - We need to count the number of ways to choose \( k \) elements from \( n \) elements, allowing for repetitions and ignoring the order of selection.

2. **Transformation to Stars and Bars:**
   - This problem can be transformed into a "stars and bars" problem. We need to distribute \( k \) indistinguishable items (stars) into \( n \) distinguishable bins (elements).
   - Each bin can hold zero or more stars, and the total number of stars is \( k \).

3. **Visual Representation:**
   - Consider \( k \) stars and \( n-1 \) bars to separate these stars into \( n \) groups. For example, if \( n = 3 \) and \( k = 5 \), a possible arrangement could be:
     ```
     * | ** | **
     ```
     - This means the first element appears once, the second element appears twice, and the third element appears twice.

4. **Counting the Arrangements:**
   - We need to count the number of distinct sequences of \( k \) stars and \( n-1 \) bars.
   - The total number of symbols (stars + bars) is \( k + n - 1 \).
   - We need to choose \( k \) positions out of \( k + n - 1 \) for the stars (or equivalently, \( n-1 \) positions for the bars).

5. **Binomial Coefficient:**
   - The number of ways to choose \( k \) positions out of \( k + n - 1 \) is given by the binomial coefficient:
     \[
     \binom{n+k-1}{k} = \frac{(n+k-1)!}{k!(n-1)!}
     \]

### Conclusion:

The general formula for the number of unordered samples of size \( k \) with replacement from \( n \) elements is indeed:

\[ \binom{n+k-1}{k} \]

This completes the proof.
