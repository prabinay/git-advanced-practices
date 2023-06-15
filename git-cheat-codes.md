# Cheat sheet
Now it's time for you to practice Trunk-Based Development on your own. By playing a few more rounds of GitHub Minesweeper you have the chance to build up muscle memory. It might feel cumbersome at first. But believe me, it'll get better soon and it'll come in handy once you start working on a team of developers.  
Since you might not remember all the commands here is a quick overview.  

## GitHub Minesweeper rules  
Goal of the game: flag all mines  
Available commands to add to `commands.json`:  

1. clear [field]: e.g. "clear A9", clears the selected field
2. flag [field]: e.g. "flag A9", flags the selected field. Should be used when you think this field is a mine.
3. unflag [field]: e.g. "unflag A9", removes a flag from the selected field. Should be used if you mistakenly flagged a field.\
4. end: once you flagged all mines you can end the game with this command. Tara will reveal the board and create a new PR to restart the game.


## Trunk-Based Development
1. Sync the local main branch.
2. Check out a new branch from main.
3. Add new commands to commands.json.
4. Commit and push the changes.
5. Open a Pull Request.
6. Wait for the CI checks to pass.
7. Request a review by Tara.
8. Merge the PR if it was approved. If you hit a mine, restart the game by approving and merging the PR created by Tara.


## Git Cheat Sheet
Here is a list of Git commands in the order you need them for Trunk-Based Development:  

1. Check out the main branch: `git checkout main`
2. Sync the local and remote main branches: `git pull origin main`
3. Create and check out a new branch: `git checkout -b YOUR_BRANCH_NAME`
4. Commit all file changes: `git commit -a -m "YOUR_COMMIT_MESSAGE"`
5. Push the changes to the remote repo on GitHub: `git push origin YOUR_BRANCH_NAME`
