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
2. To start, create a branch: `git checkout -b file_1_feature`
3. For each paragraph in each file, replace the lorem ipsum paragraph with a quote from `./source.txt`. **Make a commit** for each paragraph replacement.

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

- Ok, phew. you've managed to pivot our business in time by making the necessary changes.
- Now, let's get back to programming quotes. 
- Merge your features on `file_1_feature` branch onto `master` branch and push your changes. 

Let's show our team our awesome new features!
