# Prerequisite Quest

Your objective:

你的目標：

> Make all checks green.
>
> 讓所有檢查都變綠。

Rules:

規則：

- Fork this repository.
  Fork 這個 repository。
- Work on your fork.
  在你自己的 fork 上作業。
- Do not modify `.github/workflows/quest.yml`.
  不要修改 `.github/workflows/quest.yml`。
- Do not modify test expectations (`app/test.janet`) or mission fixtures just
  to make checks pass, unless a mission explicitly asks you to edit that file.
  不要為了讓檢查通過而去改測試的預期結果（`app/test.janet`）或任務的
  fixture 檔案，除非某個任務明確要求你編輯那個檔案。
- Use any tools or references you normally use while developing — Google,
  man pages, Stack Overflow, LLMs, a friend. That's all fair game.
  你平常開發時會用的任何工具或參考資料都可以用：Google、man page、
  Stack Overflow、LLM、朋友，通通合法。
- Understand every change you commit.
  理解你 commit 的每一個改動。

Start here:

從這裡開始：

→ [`QUEST.md`](QUEST.md)

## Installing Janet

## 安裝 Janet

Mission 04 runs a small [Janet](https://janet-lang.org/) program. You
have three options, and any of them is fine:

任務 04 會執行一個小小的 [Janet](https://janet-lang.org/) 程式。你有
三種選擇，任何一種都可以：

- **Install it locally** — see the
  [Janet install docs](https://janet-lang.org/docs/index.html).
  Package managers carry it too (`brew install janet`,
  `apt install janet`, `pacman -S janet`); versions vary, which doesn't
  matter for this quest.
  **在本機安裝**：參考 [Janet 安裝文件](https://janet-lang.org/docs/index.html)。
  套件管理器也有（`brew install janet`、`apt install janet`、
  `pacman -S janet`）；版本各有不同，但對這個任務來說沒有影響。
- **Use Docker instead** — Mission 05 builds an image with Janet in it
  and runs the same `app/main.janet`.
  **改用 Docker**：任務 05 會建立一個內含 Janet 的 image，並執行同一個
  `app/main.janet`。
- **Lean on CI** — push and read the Actions output. Slowest feedback
  loop of the three, but it works.
  **交給 CI**：push 上去，然後看 Actions 的輸出。三者之中回饋最慢，
  但確實可行。

`./scripts/doctor.sh` tells you what you currently have.

`./scripts/doctor.sh` 會告訴你目前的機器上有哪些東西。

Instructors: see [`INSTRUCTORS.md`](INSTRUCTORS.md).

教師請看 [`INSTRUCTORS.md`](INSTRUCTORS.md)。
