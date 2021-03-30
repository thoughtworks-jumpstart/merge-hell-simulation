# Merge Hell Simulation

In this exercise, we are all working in groups of 3, one 1 single repository on GitHub. Our job is to replace all the lorem ipsum paragraphs with quotes listed in `./source.txt` We will pair up and make changes according to the instructions below, and experience merge hell for ourselves!

### Getting started

1. One member of the group will fork this repo
1. The other members request to be added as collaborator on the project

### Part 1: merge hell across team members

- For part 1, change only files in directory_1
- For each paragraph in each file, replace the lorem ipsum paragraph with a quote from `./source.txt` **in random order**. **Make a commit** for each paragraph replacement.
- Keep going until every paragraph in the file_1.txt is replaced
- Do the same for file2.txt
- Do the same for file3.txt
- Finally do a git push
- First person to push wins! ;)
- The other members need to do `git pull --rebase` resolve the merge conflict, `git add` and `git rebase --continue`

### Part 2: merge hell across branches

1. For part 2, change only files in directory_2
1. To start, create a local branch: `git checkout -b feature/<your-name>`
1. For each paragraph in each file, replace the lorem ipsum paragraph with a quote from `./source.txt`. **Make a commit** for each paragraph replacement.
1. After you have made all the commits on your feature branch, do `git checkout master`
1. `git merge feature/<your-name>` to merge your feature branch into your local master branch.
1. Push to remote master branch. `git push`.

If someone else has already pushed to the remote master branch, you will not be able to proceed with the git push. In this case:

1. Do a `git pull`.
1. Fix the merge conflicts and `git add .`
1. Using this method, we will create a merge commit. `git commit` to complete the merge
1. Push the changes to the remote master branch `git push`

### Part 3

- There is an urgent feature release that needs to be done on master. We're changing our business model from serving programming quotes to serving general inspirational quotes
- Here's what you need to do:
  - checkout to master `git checkout master`
  - Update file_1 with the following content:

```
<directory_2/file_1.txt title>

The best revenge is massive success. –Frank Sinatra

People often say that motivation doesn’t last. Well, neither does bathing.  That’s why we recommend it daily. –Zig Ziglar

Life shrinks or expands in proportion to one's courage. –Anais Nin
```

- Add and commit
- `git push`
- Ok, phew. you've managed to pivot our business in time by making the necessary change.
