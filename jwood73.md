 # Profile: [Jaevon Woods]

- **NetID:** [jwood73]
- **Major:** [Mathematical Computer Science]
- **Question that I chose from the memoization exercise:** Count ways to reach the n'th stair
- **Link to the question article:** (https://www.geeksforgeeks.org/dsa/count-ways-reach-nth-stair/)

- **My solution:**
    if (n == 0 || n == 1)
        return 1;

    return countWays(n - 1) + countWays(n - 2); // i noticed the pattern was similar to the fibonacci sequence
                                                // and how the # of ways to reach the stairs would increase by 1 and be odd if n was even
}

int main() {
    int n = 4;
    printf("%d", countWays(n));
    return 0;
}
