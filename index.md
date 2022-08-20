# Welcome to my Portfolio!
My name is Devon Jarman. I am a Senior in College and getting my Bachelor's in Computer Science. In my Software Engineering class I did four projects where I learned a lot and made some cool things. Here are my assignments.
### Hangman
This assignment was an online hangman game. This game was developed using php code. This was my first time using php. It was a challenge, but rewarding. Way better than javascript. This page has a login system that has password hashing and salting. This form of encryption helps to preserve user data. The login system also checks to verify user credentials. When creating an account the user is asked to enter username and password. The password has a confirmation that must mathch. I used infinty free as the server to the game. There is a database used to save user data, words to be guessed, and also highscores for each word length. The user can login into their account or create an account. After logging in, the user is taken to the game where they can play and guess letters until the word is guessed. They then go to a highscores tables, showing them the scores for that length of word. 
This block of code is the user credential authentication. It rehashes the password to check against the database to allow the user to login.

```
 $row = $result->fetch_assoc();
		$salt = $row["Salt"];
        $hash = $row["Hash"];
        //use sha256, hash the pass + salt
        $test = hash("sha256", $pass . $salt);
        if($test === $hash) {
            $sql = "SELECT Word, Length FROM Wordlist ORDER BY RAND() LIMIT 1;
```
            
\
[Play Hangman](https://thejarman.epizy.com/Welcome.php)
\
[Hangman Github](https://github.com/thejarman1/Hangman)
### Banking App
### Stock Investing Game
### Boggle
