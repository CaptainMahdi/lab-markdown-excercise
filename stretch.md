Mahdi Hteit 7/2/2025

# What I Learned Today
- I learned about common crawl 
- I learned Fine Web uses cleaning for the websites filtering:
	1. URL Filtering: Removes spam sites, abusive and irrelevant sites
	2. Language Filtering: Keeps only English
	3. PII Removal: Removes personal info
- Computers ***cant understand raw text*** so they have to use **tokens**
- Tokens are chunks of texts resembled by:
	- #tokens
	- Binary (but it was quickly proven **inefficient**)
	- Byte Pair Encoding, which is used to make the sentences *shorter* allowing *easier* *access*
	- 100,277 is the highest BPE characters that has been used so far.
	- ![Image of tokens compared to scentences](https://miro.medium.com/v2/resize:fit:709/1*XAb4MS1zYKPcO_r-G_fUzQ.png)
- Models can output a probability distribution to determine what the next token will be using weights
- Weights are numbers that control how much influence one token has on predicting the next token.
- They use matrix multiplication which is a basis on how weights and inputs combine.
- Models are ***stochastic*** which means its random and it wont give you the same output every time!

## Lab Reflection
#troubling #tokens 
> - Understanding the BPE is very hard for me since it I'm the kind of person who needs to know why something works. But there's no way to understand why all **100,277** tokens are corresponding to certain characters.


## Code Snippet
#troubling 

```while playagain == "y"
    
    mode = input("Choose a mode: Easy, Medium, Hard, or Expert: \n").lower()

  

    if mode == "easy":
        compguess = random.randint(1, 10)
        range = 10
    elif mode == "medium"
        compguess = random.randint(1, 20)
        range = 20
    elif mode == "hard":
        compguess = random.randint(1, 50)
        range = 50
    elif mode == "expert":
        compguess = random.randint(1, 100)
        range = 100
    else:
        print("Invalid mode")
        exit()

  
    guess =int(input(f"Guess which number I'm thinking of between 1 and {range}: \n"))

  

    if guess == compguess:

        print("YOU GOT IT")

        streak += 1

    elif guess > compguess:

        print(f"Too high, the number was {compguess}")

        streak = 0
    elif guess < compguess:

        print(f"Too low, the number was {compguess}")

        streak = 0

    print(f"Good Game! Your streak has changed to, {streak}")
    playagain = input("Do you want to play again? (Y/n): ").lower()'''

## Helpful Links
[Tiktokenizer](https://tiktokenizer.vercel.app/?model=cl100k_base)
[Hyperbolic](https://app.hyperbolic.ai/models)



