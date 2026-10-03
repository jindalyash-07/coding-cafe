# Lab 4 Answers

## Question 1
`--global` means the setting applies to Git for my user account across all repositories on this computer. If I leave it out, the setting applies only to the current repository.

## Question 2
`ls -a` showed the hidden `.git` directory, which is not normally shown by `ls`. It contains Git's internal repository information, including the history, configuration, references, and other data Git needs to manage the project.

## Question 3
Git was offering to track roughly 2 entries: `README.md` and the `week02/` folder. The `.venv` folder appeared in `ls -a`, but Git was not listing it as untracked.

## Question 4
Nothing disappeared from the untracked list because `.venv` was already not being shown by Git. The new `.gitignore` file appeared as an untracked file.

## Question 5
`.gitignore` should be committed because it is part of the project's configuration and tells Git which files should be ignored. If we ignored `.gitignore` itself, other people using the repository would not get the same ignore rules.

## Question 6
`README.md` moved from "Untracked files" to "Changes to be committed." In the three-places model, this means I moved the file from my working directory into Git's staging area using `git add`.

## Question 7
Git reported that 4 files changed, with 70 insertions. The four files were `.gitignore`, `README.md`, `week02/lab01-log.txt`, and `week02/notes.md`.

## Question 8
The first seven characters of my commit hash are `31a695d`. They are the shortened form of the commit's unique hash, which Git uses to identify that specific commit.

## Question 9
The four steps are edit, stage, commit, and repeat. I edit a file, use git add to stage the changes, use git commit to save them in the repository, and repeat the process whenever I make another change.

## Question 10
README.md has a special name because GitHub automatically displays it as the main introduction to a repository. It is placed in the repository's top-level directory so visitors can see it immediately when they open the repository.

## Question 11
`gh auth login` authenticated my GitHub account and stored the credentials for Git to use. Because Git is authenticated, I do not need to enter my GitHub password every time I push.

## Question 12
The `README.md` file is showing on the front page of the GitHub repository. GitHub automatically renders README.md as the main introduction to a repository.

## Question 13
No, pushing did not change my local history. `git push` only copied my existing local commits to GitHub; the commits and their hashes remained the same.

## Question 14
A private repository exists on GitHub but its contents can only be accessed by people who have permission, such as invited collaborators. A repository that does not exist on GitHub has no online repository for anyone to access or collaborate on.
