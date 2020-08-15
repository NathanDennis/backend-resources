## Linux Learning Resources

This file will be continually added to. If it gets big enough to justify splitting everything into different files and sub folders, I'll move things around

___

### Linux Command Line Basics

Some of these commands are common across different operating systems and is very beneficial to familiarise yourself with

#### cd
- Change your current directory
- Move within your current working directory, or specify a path to change to

Example: 

`cd ../` - move up one folder to the parent folder

`cd /usr/local` - move into the folder named 'local' inside the 'usr' directory

#### ls
- List the contents of the current directory

Example:

`ls` - By itself will list the contents of the folder you are in

`ls -1` - List folder contents in a single column list

`ls` Has a lot of optional flags - [More examples here](https://www.howtogeek.com/448446/how-to-use-the-ls-command-on-linux/)

___

### File reading and output redirection

Commands related to the reading of file contents, output redirection and manipulation of folders

#### head
- Read only the first 10 lines (by default) of a file
- Can use an argument to specify how many lines to output

Example:

`head video_games.tsv` - Outputs the first 10 lines of the file named `video_games.tsv`

`head -3 package.json` - Outputs the first 3 lines of the `package.json` file

#### tail
- Similar to `head` but outputs the *last* 10 lines of a file by default
- Can also use a number argument to specify the number of lines to display

Example:

`tail package.json` - Outputs the last 10 lines of `package.json`

`tail -15 package.json` - Outputs the last 15 lines of `package.json`


#### mv
- Rename a directory

Example:

`mv components pages` - In the current directory, rename the folder called `components` to `pages`

#### curl
- Fetch the source contents of a URL and output them to the console
- Can use output redirection to store contents in a file

Example:

`curl https://www.google.com` - Fetches the page source of google.com and outputs the result

`curl https://www.google.com > google.txt` - Fetches the page source and writes the result to a file called `google.txt`. If the specified file doesn't exist, it is created and then written to

#### file
- Describe a file's type and other details

Example:

`file google.txt` - Describes a file called google.txt with the output of:

- `google.txt: HTML document, ISO-8859 text, with very long lines`

#### grep
- Search a file for a pattern of text and return matching results
- Follows the syntax of `grep OPTIONS PATTERN FILE`

Example:

`grep "google" google.txt` - Searches the google.txt file for case sensitive matches of "google" and outputs the results
`grep -i "google" google.txt` - Searches for case *insensitive* matches of "google", including "Google", and outputs the results
