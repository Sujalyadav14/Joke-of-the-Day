# Joke-of-the-Day
Tells Joke
My dApp is a Joke of the Day built on Algorand. Create a solid README.md with:

- Project Description  
- What it does  
- Features  
- Deployed Smart Contract Link: Joke of the Day
Use this code:  
//paste your code  

README should be beginner-friendly, and attractive for GitHub. Keep placeholders (Joke of the Day and //import { Contract,GlobalState } from '@algorandfoundation/algorand-typescript'


// Joke of the Day Contract
export class JokeOfTheDay extends Contract {

  // Store the joke in global state
  joke = GlobalState<string>({ key: "joke", initialValue: "" });

  // Add a new joke
  AddJoke(newJoke: string): string {
    this.joke.value = newJoke;
    return "Joke updated!";
  }

  // Retrieve the current joke
  GetJoke(): string {
    return this.joke.value;
  }
}
) as is.
