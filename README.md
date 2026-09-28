# Group 7 – Hashing Assignment

## Assignment Question 7

A music application stores the following song IDs:

`105, 210, 315, 420, 525, 630, 735, 840`

This project implements:
- Hash table using the Division Method
- Insertion of all given song IDs
- Collision detection
- Hashing search
- Linear search
- Counting operations/comparisons for both searches
- Load-factor calculation
- Comparison with theoretical time complexity
- Conclusion on suitability of hashing for the application

## Files

- `group7_hashing.c` – Complete C program
- `REPORT.md` – Assignment report with algorithm, complexity analysis, sample results and conclusion
- `SAMPLE_OUTPUT.txt` – Example execution
- `.gitignore` – Basic Git ignore file

## How to compile

Using GCC:

```bash
gcc group7_hashing.c -o group7_hashing
```

## How to run

Linux/macOS:
```bash
./group7_hashing
```

Windows:
```bash
group7_hashing.exe
```

The program automatically builds the hash table and then allows searches. It also demonstrates searches for present and absent IDs.

## Hash function

The Division Method is:

`h(key) = key % TABLE_SIZE`

A table size of 11 is used. Since the supplied IDs are multiples of 105, this produces several collisions, making the collision behaviour easy to observe.

Linear probing is used to resolve collisions.

## Important

The program is self-contained and requires only a standard C compiler.
