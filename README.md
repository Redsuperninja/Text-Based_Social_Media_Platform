# Text-Based Social Media Platform

A command-line social media simulator in C++17, built as the final project for CSCI 2270 (Data Structures) at CU Boulder. It loads real tweet data from CSV and stores it in hand-written data structures:

- a **min-heap** (`minHeapify.*`) ordered by posting time, built over all loaded tweets
- a **chained hash table** (`hash.*`) keyed by username, holding each user
- a **binary search tree** per user (`bst.*`) holding that user's posts, used to find each user's most-liked post

From the menu you can add users and posts, list all tweets or users, show one user's posts, find the most-liked post, and print performance metrics comparing the structures.

## Build and run

```bash
make run_small   # builds and runs on datasets/test.csv
make run_big     # larger dataset: datasets/tweets-data_smol.csv
```
