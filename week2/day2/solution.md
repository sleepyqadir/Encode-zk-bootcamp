
# Homework 5

1. Recursion example: <br/>

    ![Screenshot from 2022-10-06 15-18-45](https://user-images.githubusercontent.com/38910854/194288758-3780d59f-bca3-46c7-a02c-b93f8860b1af.png) 

<br/> <br/>

**recursion exercise solution:** [ExtropyIo cairo recursion exercises](https://github.com/sleepyqadir/ZeroKnowledgeBootcamp/blob/main/starknet/exercises/cairo/ex4.cairo)


2. Does this example use tail recursion: <br/>

    no the recursion example does'nt use the tail recursion as the every recursion call has to complete before cairo compiler calculates the sum. for example: <br/>

    ```
    compute_sum(5)
    5 + compute_sum(4)
    5 + (4 + compute_sum(3))
    5 + (4 + (3 + compute_sum(2)))
    5 + (4 + (3 + (2 + compute_sum(1))))
    5 + (4 + (3 + (2 + (1 + compute_sum(0)))))
    5 + (4 + (3 + (2 + (1 + 0))))
    5 + (4 + (3 + (2 + 1)))
    5 + (4 + (3 + 3))
    5 + (4 + 6)
    5 + 10
    15
    ```


3. How does Argent account differ to an Ethereum EOA:

Argent accounts are contract accounts, which are controlled by their contract code. While Externally Owned Accounts (EOA) are controlled by private keys.


