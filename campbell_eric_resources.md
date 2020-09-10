Pro Git Book

copy current full path
pwd|pbcopy

make sure you have all ownership
sudo chown -R $(whoami) /usr/local/*
  obv change the path to wherever is needed

delete through all permissions (requires my password)
sudo rm -rf /usr/local/include/node
  obv change path as needed

use as super user
sudo su

find a file
find / -name <the name here> -print

hide all desktop icons!!!
defaults write com.apple.finder CreateDesktop -bool false
killall Finder
(run this on two separate lines)

to put desktop icons back
defaults write com.apple.finder CreateDesktop -bool true
killall Finder

great resource for homebrew things!
https://discourse.brew.sh/

https://chris.beams.io/posts/git-commit/

good commit msg shows whether developer good collaborator
  re-establishing context code wasteful
  reduce as much as possible

git log
  git blame
  revert
  rebase
  log
  shortlog

"commit squashing"

teams should agree commit msg convention defines at least these three things
  * style
    simple is best
  * content
    what info should contain, should NOT contain
  * metadata
    how to handle issue tracking IDs, pull request numbers

best to write commit messages in a text editor

Seven Rules of a Great Commit Message!

1. Separate subject from body with a blank line

2. Limit the subject line to 50 characters
forced to think most concise way get point across

3. Capitalize the subject line

4. Do not end the subject line with a period

5. Use the imperative mood in the subject line

6. Wrap the body at 72 characters

7. Use the body to explain what and why v. how


The "Atomic Approach"
commit each fix or task as a separate change
only commit when a block of work is complete
commit each layout change separately
joint commit for layout file, code behind file, and additional resources

Benefits of the "Atomic Approach"
easy to roll back without affecting other changes
easy to make other changes on the fly
easy to merge features to other branches

Rule of thumb: correct msgs can read this way
"If applied, this commit will ___"

need to wrap msgs at 72 characters
  (need to figure out what this means)

focus making clear the reasons why made change
  way worked before
    what was wrong with that/
  way works now
  why solved that way

don't forget tab completion to help remember all the git commands!

Interesting ways to use git
git-format-patch(1) turns commit into an email


New git commands
git show
git log -p
git log --oneline (prints out just the subject line)
git rm



More git resources
https://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration - git configuration stuff that can help
https://www.freshconsulting.com/atomic-commits/ - da fuq is an atomic commit?!
https://sandofsky.com/workflow/git-workflow/
http://svnbook.red-bean.com/en/1.7/svn.branchmerge.commonpatterns.html
https://app.pluralsight.com/player?name=6eec00f4-f910-4efc-9698-936948026502&mode=live&clip=0&course=code-school-git-real&author=gregg-pollack
https://www.codecademy.com/pt-BR/learn/learn-git
https://lab.github.com/
