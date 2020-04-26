# Letter Checker
A little app to calculate the score of a letter sent in Animal Crossing : New Leaf.


## ACNL Letter Checks
Following info is quoted from this [article](https://www.polygon.com/2018/8/7/17660344/animal-crossing-letter-system-game-design-explained) and these [tweets](https://twitter.com/jamchamb_/status/1025977659522789376). 
<ol type="A">
  <li>looks out for punctuation and capital letters. Having a punctuation mark at the end of the letter grants 20 points, and every punctuation mark before that must be followed by a capital letter within three spaces, earning or losing 10 points depending.</li>
  <li>checks for common trigrams (three-letter groups) from a table. The total number of trigrams multiplied by three is added to the score.</li>
  <li>makes sure that the first character in the letter is capitalized. If it is, that’s 20 points. If not, it costs 10.</li>
  <li>looks for repetition — if a letter is repeated three times in a row, it docks 50 points and stops checking.</li>
  <li>gets a little fancy and checks for the ratio of spaces to non-spaces in the letter. If there’s only spaces or if the ratio of spaces to other characters is less than 20, then the letter loses 20 points. Otherwise, it gains 20.
</li>
  <li>only occurs if the letter is more than 75 characters long. If it is and has no punctuation for at least 75 more characters, then the score gets a whopping 150-point deduction.</li>
  <li>checks each group of 32 characters for at least one space. Every time that doesn’t occur, it deducts 20 points.</li>
</ol>

A “good” letter has a score of 100 or above, and a “bad” letter has one of 50 or below.

Getting special replies with gifts is another rank-system that’s only based on the trigram counts and repeating characters. Up to two points are awarded to the rank, depending on the trigram percentage, and three more if there are no non-space characters repeated more than three times. If there’s a present attached, six points are rewarded. If the total rank is above three, you’ll get a gift in the reply; each level above three comes from a different group of items.

## References
1. https://www.polygon.com/2018/8/7/17660344/animal-crossing-letter-system-game-design-explained
2. https://twitter.com/jamchamb_/status/1025977659522789376

Same idea: https://acletter.000webhostapp.com/
