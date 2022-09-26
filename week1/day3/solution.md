
# Homework 3

## Practice using Zokrates

1. Use the example file to generate a proof to show that a prover knows the square root
of 25.

<br/>

  **Solution gist:** [square root
of 25](https://gist.github.com/sleepyqadir/8a39b2389e2fd94f0f68b862dc8b5520)

<br/>

  **Valid proof screenshot**
<br/>

![Screenshot from 2022-09-23 16-42-08](https://user-images.githubusercontent.com/38910854/192204364-f070d0d2-26ed-4125-a4b3-2a80546a1332.png)

<br/>
<br/>


2. Create an invalid proof and make sure it is rejected <br/>
<br/>


  **Invalid proof screenshot**
<br/>

![Screenshot from 2022-09-23 16-42-47](https://user-images.githubusercontent.com/38910854/192204378-53672742-8043-4e60-a06d-c989f78cb898.png)

<br/>
<br/>


3. Follow the example to build a proof that you know the pre pre image of a hash
<br/>


  **Solution gist:** [Proving pre image of hash](https://gist.github.com/sleepyqadir/a6ec6564da582b757bb115c7592d8722)
<br/>


  **Valid proof screenshot**
<br/>

![Screenshot from 2022-09-26 12-29-52](https://user-images.githubusercontent.com/38910854/192218616-ca9b4a44-0bb2-46d1-8deb-c3abbf318855.png)
<br/>


  **Invalid proof screenshot**
<br/>

![Screenshot from 2022-09-26 12-31-24](https://user-images.githubusercontent.com/38910854/192218664-a61db3f9-13d9-4654-9970-db3138c02234.png)


<br/>
<br/>

4. In principle how could you use Zokrates to verify that a certain address on Ethereum
has more than say 1 ETH ?




  We can do this by designing a circuit with a single public input. The circuit will check that the input value is equal to:

  ```
  assert( value == 1000000000000000000)
  ```

    The input value should be equal to 1e18. 
    
  One thing we must ensure while verifying the certain address balance using this circuit is that the user's balance is directly taken from the smart contract, not from the user.


