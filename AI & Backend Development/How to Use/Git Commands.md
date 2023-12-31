
# Git on VSC

## Git?

[Git.md](../../1일차/03.Git.md)

## With Visual Studio Code GUI

### 0. 깃허브 원격 저장소 생성하기

https://github.com/ 에서 ReadMe.md, .gitignore 를 추가하지 않은 완전히 비어있는 원격 저장소를 생성한다.
비어있는 원격 저장소가 이미 존재한다면 그대로 사용하여도 된다.
아래는 비어있는 원격 저장소를 생성하였을 때 안내되는 터미널 커맨드를 따라 Visual Studio Code 에서 Git 을 사용하는 방법이다.

### 1. Initialize Repository

- GUI

Find Source Control|Press Initialize Repository
---|---
![](https://github.com/nhn-academy-marco/nhn-academy-dev-settings/blob/8039b0b211c749a4de378433234e4e628ac6be2d/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/01.find-source-control.png)|![](https://github.com/nhn-academy-marco/nhn-academy-dev-settings/blob/8039b0b211c749a4de378433234e4e628ac6be2d/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/02.source-control-gui.png)
- Command

```terminal
git init
```
src
### 2. Add File
- GUI

![](https://github.com/nhn-academy-marco/nhn-academy-dev-settings/blob/8039b0b211c749a4de378433234e4e628ac6be2d/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/03.add-file.png)
- Command
```
git add src/App.java
```

### 3. Commit changes

#### Try Commit

- GUI

![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/04.commit-changes.png)

- Command

```
git commit -m "add source App.java"
```

#### Set Git User info

- GUI

![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/05.set-git-user.png)
![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/05-1.git-config.png)

- Command

```
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```

### 4. Push Commit

#### Try Push Commits

- GUI

![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/06.push-commit.png)

- Command

```terminal
git push ... 
```

#### Add Remote

- GUI

![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/07.set-remote.png)

![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/09.set-remote-url.png)

![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/10.set-remote-name.png)

- Command

```
git remote add origin https://github.com/devel0624/vsc-test-repository.git
```

#### Remane Branch

- GUI

![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/11.make-branch.png)
![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/13.set-branch-name.png)


- Command

```
git branch -m main
```

#### Retry Push

- GUI

![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/14.try-push.png)|![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/15.publish-branch.png)
-|-

- Command

```
git push origin main
```


### Commit From Remote

![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/16.check-remote.png)|![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/17.add-new-file.png)
-|-
![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/18.write-readme.png)|![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/19.commit-readme.png)

### 5. Pull Remote Commits

#### Fetch Branch

- GUI

![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/20.fetch-branch.png)

- Command

```
git fetch origin main
```

#### Pull Commits

- GUI

![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/21.show-remote-change.png)|![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/22.pull-commits.png)
-|-

- Command

```
git pull origin main
```

#### Check Applies

![](https://github.com/SeinJs/nhn-academy-dev-settings/blob/main/gyeongnam-docs/2%EC%9D%BC%EC%B0%A8/00.Visual%20Studio%20Code/images/git-on-vsc/23.apply-commit.png)
