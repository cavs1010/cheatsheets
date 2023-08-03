# Git Cheatsheet 📚

This is a simple guide or 'cheatsheet' to help you understand and use Git. We'll cover what Git is, how to save changes, work with branches, merge code, and use Git commands in the terminal. Let's get started! 😄

## Git: What is it? 🤔
Git is like a time machine 🕰️ for your code. It remembers all the changes you've made, so you can go back to any point or see what others have changed. Plus, it lets you work on different versions of your code at the same time without mixing them up!

## Commits: Saving Changes 📝💾
In Git, 'saving' your changes is called a 'commit'. It's like taking a snapshot 📸 of your code at a certain moment.

~~~
# Let's make a change to our code and save it
echo "print('Hello, world!')" > hello.py
git add .
git commit -m "My first commit"
~~~

## Branches: Trying New Things Safely 🌳
A 'branch' in Git is like an alternate reality for your code. It lets you try new ideas 💡 without messing up your main code. Once you're happy with your changes, you can bring them back into your main code.

~~~
# Let's make a new branch and switch to it
git branch my-branch
git checkout my-branch
~~~

## Merging: Bringing Changes Together 🤝
'Merging' in Git is how you bring changes from one branch back into your main code. It's like weaving two threads together.

~~~
# Let's bring the changes from my-branch back to the main code
git checkout main
git merge my-branch
~~~

## Using Git in the Terminal 🖥️🔡
You can use Git commands in the terminal to manage your code. Here are some of the most common ones:

~~~
# See which files have changed
git status

# Add all changes to be saved
git add .

# Save changes with a message
git commit -m "<Your message>"

# Send changes to the main code on GitHub
git push origin main
~~~
