## File reading and output redirection

Commands related to the reading of file contents, output redirection and manipulation of folders

### head
- Read only the first 10 lines (by default) of a file
- Can use an argument to specify how many lines to output

Example:

- `head video_games.tsv` - Outputs the first 10 lines of the file named `video_games.tsv`
- `head -3 package.json` - Outputs the first 3 lines of the `package.json` file

### tail
- Similar to `head` but outputs the *last* 10 lines of a file by default
- Can also use a number argument to specify the number of lines to display

Example:

- `tail package.json` - Outputs the last 10 lines of `package.json`
- `tail -15 package.json` - Outputs the last 15 lines of `package.json`


### mv
- Rename a directory

Example:

`mv components pages` - In the current directory, rename the folder called `components` to `pages`



