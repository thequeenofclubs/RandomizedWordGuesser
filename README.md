# RandomizedWordGuesser
RandomizedWordGuesser is a simple word game that runs in your terminal.
> Installation Instructions are located at the bottom of this file.


## Usage
To launch the game, type rwg in your terminal. Once the game is launched you will see instructions for how to play.

Your goal is to guess the correct word given that same word with its letters in random order.  
For example, if the correct word is grapes, you may be given any combination of those letters, one of which could be paserg.  
You would then have to piece together the original word. You get as many guesses as you like.  
The game will then wait for your first guess. If you do not get the correct answer, the game will inform you and prompt you for your next guess.z

If you would like to give up, you can type ``igiveup`` as your guess.

### Debug Tools
#### Show Answer
Type ``debugshowanswer`` as your guess to force the game to show you the correct answer.

#### Show Codes
Type ``debugshowcodes`` as your guess to show the list of exit codes that the program can produce.

| Error Code | Meaning                                                                     |
| ---------- | --------------------------------------------------------------------------- |
| Code 0     | The Player has guessed the correct answer and doesn't want to play anymore. |
| Code 2     | The player did not guess the correct answer and has chosen to give up.      |

## Installation
### Method 1: Install VSH
RWG is bundled with VSH, which has a dedicated install script which simplifies the installation process substantially. You can install VSH by [visiting it's repo](https://github.com/thequeenofclubs/vsh) and following the instructions there.


### Method 2: Manual Installation
If you don't want to install VSH, you can run RWG from within BASH or ZSH by installing it manually.
**Steps:**
1. Download the RWG executable from the releases page.
2. Create a folder in your home folder called ~/Scripts
3. Add the scripts folder to the path by typing ``export PATH=$PATH:~/Scripts``.
4. Move the RWG executable into the Scripts folder you just created.
5. Create a folder within ``Scripts`` called ``rwglib`` (Case Sensitive)
6. Copy the ``words.dat`` file into the ``rwglib`` folder you just created.
7. Restart your shell for the changes to take effect.
