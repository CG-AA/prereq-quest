# The Quest

## The spirit of this

## 這份問卷的精神

This is a survey, not a test. It exists so we can understand how you
actually do things. So:

這是一份問卷，不是考試。它的目的是讓我們了解你平常實際上是怎麼做事
的。所以：

- **Do it the way you'd normally do it.** Same tools, same habits, same
  shortcuts.
  **照你平常的方式來做。** 一樣的工具、一樣的習慣、一樣的捷徑。
- **Don't put extra effort into this.** Don't study for it, don't polish
  it, and don't grind through a mission you can't crack.
  **不要為此多花額外的力氣。** 不用為它預習，不用把它打磨得很漂亮，
  也不要硬啃一個做不出來的任務。
- **Every answer is welcome.** "I don't know" and "I gave up here" are
  perfectly good answers, and they tell us more than a copied solution.
  **每一種回答都歡迎。** 「我不知道」和「我在這裡放棄了」都是很好的
  回答，而且比抄來的解答更能告訴我們事情。

Welcome. This repository is a small diagnostic, not an exam. It exists so
you and your TA can see what you're already comfortable with, and
what's worth practicing before the term gets going.

歡迎。這個 repository 是一個小型的診斷，不是考試。它的目的是讓你和
你的助教看見你已經熟悉哪些東西、哪些值得在學期開始前先練習。

There is no single score at the end. Instead, GitHub Actions will build a
capability profile from what you actually did — separate from anything
you self-report.

最後不會有一個單一的分數。取而代之的是，GitHub Actions 會根據你實際
做了什麼，建立一份能力側寫，和你自己填寫的自評是分開的。

## How this works

## 流程說明

1. Fork this repository to your own GitHub account.
   把這個 repository fork 到你自己的 GitHub 帳號。
2. Clone your fork locally.
   把你的 fork clone 到本機。
3. Work through the missions below, roughly in order.
   大致依照順序完成下面的任務。
4. Commit as you go (see Mission 02 — this matters).
   邊做邊 commit（見任務 02，這很重要）。
5. Push to your fork.
   Push 到你的 fork。
6. Open the **Actions** tab on your fork and read the results. The first
   time, GitHub asks you to enable workflows on your fork — until you
   click enable, pushes will appear to do nothing. Enabling doesn't
   re-run anything by itself: push again, or use the manual
   **Run workflow** button on the `quest` workflow.
   打開你 fork 上的 **Actions** 分頁，讀取結果。第一次進去時，GitHub
   會要求你在 fork 上啟用 workflow；在你按下啟用之前，push 看起來
   會像什麼都沒發生。啟用本身不會重新執行任何東西：再 push 一次，
   或是在 `quest` workflow 上按手動的 **Run workflow** 按鈕。
7. Keep pushing fixes until the checks are green.
   持續 push 修正，直到檢查全部變綠。

If you get stuck on *how* to fork, clone, commit, or push — that's fine.
Figuring that out is itself part of what this diagnostic measures. Use
whatever you'd normally use to figure it out.

如果你卡在*怎麼* fork、clone、commit 或 push，沒關係。把這些弄懂本身
就是這個診斷要衡量的一部分。用你平常會用的任何方法去弄懂它。

## If you get stuck

## 如果你卡住了

Give it about 10 focused minutes with your usual resources first —
error messages, search, docs, an LLM, a classmate. If you're still
stuck after that, **message your TA directly** and describe
what you were trying to do, what you ran, and what happened instead.

先用你平常的資源專注試個 10 分鐘左右：錯誤訊息、搜尋、文件、LLM、
同學。如果之後還是卡住，**直接私訊你的助教**，描述你想做什麼、你
執行了什麼，以及實際發生了什麼。

Whatever happens, don't sink more than about **90 minutes** total into
this quest. If you find yourself struggling, or you've passed that
mark, **report back to the TA before trying any further.** You are not
expected to finish everything.

不管怎樣，整個任務加起來不要花超過 **90 分鐘**。如果你發現自己很吃力，
或是已經超過這個時間，**請先回報給助教，再決定要不要繼續嘗試。** 我們
並不期待你把所有東西都做完。

Getting stuck is data, not a penalty. Where a cohort gets stuck is
exactly what this diagnostic is for, and a clear description of a wall
you hit is worth more than silently giving up on a mission.

卡住是資料，不是扣分。一整屆學生會卡在哪裡，正是這個診斷想知道的；
清楚描述你撞到的牆，比默默放棄一個任務更有價值。

## Before you start

## 開始之前

Run the doctor script to see what's available on your machine:

執行 doctor 腳本，看看你的機器上有哪些東西可用：

```console
./scripts/doctor.sh
```

On **Windows**, run this (and everything else here) from **Git Bash**,
which ships with Git for Windows, or from WSL. These are shell scripts;
PowerShell and `cmd` can't run them.

在 **Windows** 上，請用 **Git Bash**（隨 Git for Windows 一起安裝）
或 WSL 來執行這個腳本以及這裡的所有其他東西。這些都是 shell script，
PowerShell 和 `cmd` 跑不動。

Nothing here needs to be installed system-wide except Git. Docker and
Janet are each used by exactly one mission, and you don't strictly need
either: see [Installing Janet](README.md#installing-janet) in the root
README for your options, one of which is letting GitHub Actions run
things for you.

除了 Git 之外，這裡沒有任何東西需要安裝到整個系統。Docker 和 Janet
各只有一個任務會用到，而且你並不一定需要它們：請看根目錄 README 裡的
[Installing Janet](README.md#installing-janet) 了解你的選項，其中之一
就是讓 GitHub Actions 幫你執行。

## Mission 00 — Who are you?

Create `answers/<your-github-username>.md` from the template at
[`answers/README.md`](answers/README.md) (or copy
[`answers/TEMPLATE.md`](answers/TEMPLATE.md) directly). Fill in the
`Environment`, `Things I have done before`, and the two free-response
sections. You'll fill in the rest of this file as you complete missions.

## Missions

| # | Mission | Focus |
|---|---|---|
| 01 | [Linux scavenger hunt](missions/01-linux/README.md) | filesystem, shell, pipes |
| 02 | [Git](missions/02-git/README.md) | commits, forks, merge conflicts |
| 03 | [SSH](missions/03-ssh/README.md) | SSH authentication / remote connection |
| 04 | [Debug](missions/04-debug/README.md) | reading unfamiliar code |
| 05 | [Docker](missions/05-docker/README.md) | containers, build/run |
| 06 | [Improve something](missions/06-improve/README.md) | judgment, initiative |

## Checking your progress

```console
./scripts/check.sh
```

runs every check that doesn't need an external server. It won't catch
everything GitHub Actions checks (Docker and Janet only run locally if
you have them installed), but it's the fastest feedback loop you have.

## The fine print

- Every check maps to something a working developer does regularly. None
  of it requires memorizing flags or trivia.
- If a check is red, the fix is almost always: read the error message
  first.
- The Actions job summary shows a capability profile, not a score. A
  `⚪ unverified` result is not a failure. SSH is *always* reported this
  way: this repository doesn't automate checking a live SSH session, so
  whether or not a server is configured, that mission is self-reported.
