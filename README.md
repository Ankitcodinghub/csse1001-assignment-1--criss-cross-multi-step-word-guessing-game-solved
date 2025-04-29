# csse1001-assignment-1--criss-cross-multi-step-word-guessing-game-solved
**TO GET THIS SOLUTION VISIT:** [CSSE1001 Assignment 1- Criss-Cross Multi-Step Word Guessing Game Solved](https://www.ankitcodinghub.com/product/csse1001-criss-cross-multi-step-word-guessing-game-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;115999&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSSE1001 Assignment 1- Criss-Cross Multi-Step Word Guessing Game Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
1 Getting Started

To start, download a1.zip from Blackboard and extract the contents. The a1.zip folder contains all the necessary files to start this assignment. Some support code has been provided to assist with implementing the tasks. You will be required to implement your assignment in a1.zip.

The other provided file is a1support.py, which contains some code to help you implement your assignment. You are not compelled to use this file to implement your assignment but it is strongly recommended. Do not make changes to the a1support.py file. The only file that you should submit is a1.zip. It could cause unexpected errors submit more than one file or if you made changes to the a1 support.py file as well.

2 Concepts

At the start of the game the user selects a difficulty, and then a word is chosen at random based on that difficulty. The word length will depend on the difficulty selected by the user; either “FIXED” (meaning the word will be exactly eight letters long), or “ARBITRARY” (meaning the word will be anywhere between six to eight letters long). The goal of the game is for the player to guess that word through a series of guesses of “subwords”. The player will have a different number of guesses (with different subwords to guess; see GUESS INDEX TUPLE), depending on the difficulty selection. If the player chooses the “FIXED” difficulty, the word must be selected at random from the WORDS FIXED.txt file. If the player chooses the “ARBITRARY” difficulty, the word must be selected at random from the WORDS ARBITRARY.txt file.

At program startup, the user is asked to specify one of three actions:

Input Action

’s’ Start game

’h’ The game rules will be printed out and then the game will commence

’q’ Quit game

Invalid command Print invalid command message (see below) and restart. “Please enter a valid command: “

Table 1: List of valid actions.

When the game is started the player should be prompted with:

&gt;&gt;&gt; “Do you want a “FIXED” or “ARBITRARY” length word?”

2.1 If the user specifies “FIXED”

The game randomly selects an eight-letter word from the WORDS.txt file and the correct guess sequence from the GUESS INDEX TUPLE tuple.

Each vowel guessed in the correct position gets 14 points. Each consonant guessed in the correct position gets 12 points. Each letter guessed correctly but in the wrong position within the substring gets 5 points. You can assume that the words do not contain repeated letters and all guesses are lowercase letters.

2.2 If the user specifies “ARBITRARY”

The game randomly selects a word from the WORDS ARBITRARY.txt file and the correct guess sequence from the GUESS INDEX TUPLE tuple.

The scoring system is the same as for the ”FIXED” word length.

2.3 Guessing procedure

2.3.1 For an eight-letter word

The user will be prompted to guess the word, step by step. The guessing procedure involves 8 steps, where the guess slices will depend on the GUESS INDEX TUPLE. At each of the 7 first steps the user guesses a subsection of the word and receives feedback (their score) for that guess. The final 8th step involves guessing the whole word. After the 8th guess, the user is informed of whether they ‘won’ (i.e. guessed the word correctly) or ‘lost’ (in which case they are told what the word was). If, at any stage, the player enters a guess that is of the incorrect length then the game should repeatedly prompt for the correct word length until the player enters a guess that matches the length of the substring to be guessed in that step.

The guessing and scoring procedure is illustrated in Table 2, for the 8 letter word, ”crushing”.

Table 2: Step by step guessing procedure for the word ”crushing”.

2.4 Game over

If the user guesses the correct word at the end of the game, the following message should be printed out:

“You have guessed the word correctly. Congratulations”.

If the user guesses the wrong word at the end of the game, the following message should be printed out:

“Your guess was wrong. The correct word was “{word}””

(Where word represents the word the player was trying to guess.)

2.4.1 Examples

Figure 1: Example of final guess.

3 Implementation

Within this section, the following variables hold meaning as defined below:

• word select: A string representing a FIXED or ARBITRARY word selection.

• guess no: An integer representing how many guesses the player has made.

• word: A string representing the word being guessed by the player.

• word length: An integer representing the length of the word being guessed by the player.

You must write the following functions as part of your implementation. You are encouraged to add your own additional functions if they are beneficial to your solution.

select word atrandom(word select)-&gt; str:

Given the wordselect is either “FIXED” or “ARBITRARY” this function will return a string randomly selected from WORDS FIXED.txt or WORDS ARBITRARY.txt respectively. If word select is anything other then the expected input then this function should return None. Hint: see a1 support.load words() and a1 support.random index()

create guess line(guess no, word length)-&gt; str:

This function returns the string representing the display corresponding to the guess number integer, guess no.

Example:

&gt;&gt;&gt; create_guess_line(2, 8)

’Guess 2 | – | * | * | * | – | – | – | – |’

display guess matrix(guess no, word length, scores)-&gt; None:

This function prints the progress of the game. This includes all line strings for guesses up to guess no with their corresponding scores (a tuple containing all previous scores), and the line string for guess no (without a score).

Return the score, an integer, the player is awarded for a specific guess. The word is a string representing the word the player has to guess. The substring to be guessed is determined by the start index and end index. The substring is created by slicing the word from the start index up to and including the end index. The guess is a string representing the guess attempt the player has made.

Example:

&gt;&gt;&gt; compute_value_for_guess(“crushing”, 0, 1, “rc”)

10

main()-&gt; None:

This function handles player interaction. At the start of the game the player should be greeted with the Welcome message. Once the guessing sequence commences the game should loop for the correct number of rounds until either the player wins by guessing the correct word or loses by guessing the incorrect word.

Hint: the main function should be your starting point but also the last function you finish implementing.

3.1 Example game

4 ASSESSMENT AND MARKING CRITERIA

4.1 Functionality Assessment

Functionality tests are automated and so string outputs need to exactly match what is expected.

4.2 Code Style Assessment

4.3 ASSIGNMENT SUBMISSION

You must submit your completed assignment electronically through Blackboard. The only file you submit should be a single Python file called a1.py (use this name – all lower case). This should be uploaded to

Blackboard&gt;Assessment&gt;Assignment 1.

5 Appendix

5.1 Welcome message

“Welcome to the Criss-Cross Multi-Step Word Guessing Game!

Enter an input action. Choices are: s – start game h – get help on game rules q – quit game:

”

5.2 Help message

“Game rules – You have to guess letters in place of the asterixis.

Each vowel guessed in the correct position gets 14 points.

Each consonant guessed in the correct position gets 12 points.

Each letter guessed correctly but in the wrong position gets 5 points. If the true letters were “dog”, say, and you guessed “hod”, you would score 14 points for guessing the vowel, “o”, in the

correct position and 5 points for guessing “d” correctly, but in the incorrect position. Your score would therefore be 19 points.” 5.3 Printing Example

Figure 2: Display for seven letter words.

Figure 3: Display for nine letter words.

Figure 4: Example where the player chooses ”s” to start the game.
