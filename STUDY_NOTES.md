notepad STUDY\_NOTES.md (to open notepad and add info)

\# CI/CD Training Notes



\## 🛠️ Essential Commands

\- `gh auth login`: Connect to GitHub.

\- `git init`: Start a local repository.

\- `npm install --save-dev jest`: Install the test framework.

\- `npm test`: Run tests locally.

\- `git add .`: Stage changes.

\- `git commit -m "message"`: Save a local snapshot.

\- `git push origin master`: Upload to GitHub.



\## 🧠 CI/CD Best Practices

\- \*\*Commit Daily:\*\* Small changes are easier to fix.

\- \*\*Fast Builds:\*\* Aim for under 10 minutes.

\- \*\*Fail Fast:\*\* Run the quickest tests first.

\- \*\*Fix Immediately:\*\* Never leave the pipeline "Red" (broken).

\- \*\*Automate:\*\* If you do it twice, write a script for it.

then this:git add STUDY\_NOTES.md

git commit -m "Add study notes"

git push origin master





This step is the "Philosophy" of CI/CD. While the previous steps were about mechanics (how to code), this step is about quality control (how to work professionally).

Here is the explanation of these best practices in simple terms:

\## 🚀 CI/CD Best Practices Explained



\* Commit often: Upload small changes every day. It's much easier to find a bug in 10 lines of code than in 1,000 lines.

\* Keep builds fast: A pipeline should be like an espresso machine, not a slow cooker. If it takes too long, people will start skipping it.

\* Automate everything possible: Human beings are great at thinking but bad at repetitive tasks. Let the computer handle the testing and moving of files.

\* Fix broken builds immediately: A "Red" pipeline is like a fire alarm. You shouldn't keep cooking; you should stop and fix the problem so the rest of the team can work.

\* Trunk-based development: Instead of working on long-lived "feature branches" for weeks, everyone merges their code into the master (or main) branch frequently to avoid "Merge Hell."



\------------------------------

\## 📋 Your "Cheat Sheet" of Commands

Since you wanted a list to save, here are the essential commands you've mastered so far:



| Command | Purpose |

|---|---|

| gh auth login | Connect your PC to GitHub. |

| git init | Start a new Git project. |

| npm install --save-dev jest | Install the testing engine. |

| npm test | Run your math tests locally. |

| git add . | Prepare files for saving. |

| git commit -m "msg" | Save a "checkpoint" of your work. |

| git push origin master | Sync your work to the cloud (GitHub). |



\## What's next?

You have the code, the tests, and the knowledge. The final step is to create the Automation Script (the .github/workflows/ci.yml file). This file tells GitHub: "Every time I push code, please start a virtual computer, install Node, and run npm test for me."

Ready to automate your first pipeline?





This step focuses on the mindset and strategy behind CI/CD. It’s not just about the tools; it’s about the habits that keep software development moving fast and safely.

Here is the list of commands we have used so far, along with the "Best Practices" from your current step, explained so you can save them for your reference.

\## 🛠️ Part 1: Your Command History (The "How-To")



| Command | Explanation |

|---|---|

| gh auth login | Authenticate: Connects your computer to your GitHub account. |

| mkdir cicd-demo \&\& cd cicd-demo | Project Setup: Creates a folder and enters it. |

| git init | Initialize Git: Starts tracking changes in the folder. |

| notepad .gitignore | Ignore Files: Creates a list of files (like node\_modules) that Git should NOT upload. |

| npm init -y | Node Setup: Creates package.json to manage your project. |

| npm install --save-dev jest | Install Testing Tool: Downloads the "Jest" framework to run your tests. |

| npm test | Run Tests: Checks your index.js logic against index.test.js. |

| git rm -r --cached . | Reset Tracking: Cleans Git's memory if you accidentally added the wrong files. |

| git add . | Stage Files: Tells Git "I want to save these specific changes." |

| git commit -m "message" | Snapshot: Saves your changes locally with a description. |

| git push origin master | Upload: Sends your local code to your GitHub repository. |



\------------------------------

\## 🧠 Part 2: CI/CD Best Practices (The "Why")

When you eventually build your automated pipeline (Step 5), these are the rules you should follow:



&#x20;  1. Commit Often: Don't wait a week to save your code. Small, daily updates are easier to test and fix.

&#x20;  2. Keep Builds Fast: If your pipeline takes 1 hour to run, developers will stop using it. Aim for under 10 minutes.

&#x20;  3. Fix Broken Builds Immediately: If the "Build" turns red (fails), stop everything and fix it. A broken pipeline blocks the whole team.

&#x20;  4. Automate Everything: If you find yourself doing a task manually more than twice (like running tests or deploying), write a script for it.

&#x20;  5. Fail Fast: Your pipeline should run the fastest tests (unit tests) first. If they fail, the pipeline stops immediately, saving time.



\## 📝 Saving this for yourself

You can copy this entire response into a file named STUDY\_NOTES.md in your project folder so you always have it!

Would you like to move to Step 5 now, where we actually write the GitHub Action script to automate your npm test?


gh repo view --web   (view and open the GitHub)


