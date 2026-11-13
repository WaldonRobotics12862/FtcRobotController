
## Pulling latest udpate from FTC 

Use following command to pull updates into master branch

```bash
git checkout master
git fetch upstream
git rebase upstream/master

# Push updates back to our master branch
git push origin master --force-with-lease
```

### Troubleshooting Steps to pull latest update

Check if upstream is already added 

```bash
git remote -v
```

This must show origin as well as upstream url like below:

```bash
origin    git@github.com:WaldonRobotics12862/FtcRobotController.git (fetch)
upstream  https://github.com/FIRST-Tech-Challenge/FtcRobotController.git (fetch)

```

if doesn't show upstream then add upstream url

```bash
git remote add upstream https://github.com/FIRST-Tech-Challenge/FtcRobotController.git
```

