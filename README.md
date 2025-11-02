
# 🌱 How to Contribute to an Open Source Project on GitHub

This guide explains step-by-step how to contribute to an open source project on GitHub — the right way!

---

## 🧭 Step 1: Fork the Repository

You **can’t push directly** to someone else’s repo unless you’re a collaborator.  
So first, **fork** the project to create your own copy under your GitHub account.

1. Go to the repository page on GitHub.
2. Click the **Fork** button (top-right corner).
3. This creates a new repo under your account:  
```

[https://github.com/](https://github.com/)<your-username>/<project-name>

````

---

## 💻 Step 2: Clone Your Fork Locally

Now, clone **your fork** (not the original repo) to your local machine.

```bash
git clone https://github.com/<your-username>/<project-name>.git
````

Then navigate into the project folder:

```bash
cd <project-name>
```

---

## 🔗 Step 3: Add the Original Repo as an “Upstream” Remote

This helps you **keep your fork updated** with the latest changes from the main project.

```bash
git remote add upstream https://github.com/<original-owner>/<project-name>.git
```

You can verify with:

```bash
git remote -v
```

You should see:

```
origin    https://github.com/<your-username>/<project-name>.git (fetch)
upstream  https://github.com/<original-owner>/<project-name>.git (fetch)
```

---

## 🌿 Step 4: Create a New Branch

Never work directly on the `main` branch.
Create a separate branch for your fix or feature:

```bash
git checkout -b feature-or-fix-name
```

Example:

```bash
git checkout -b fix-readme-typo
```

---

## 🧩 Step 5: Make Your Changes

Edit files, add features, or fix bugs.
Test your changes before committing.

---

## 💬 Step 6: Commit Your Changes

```bash
git add .
git commit -m "Fix typo in README"
```

Use clear, meaningful commit messages!

---

## 🚀 Step 7: Push Your Branch to Your Fork

```bash
git push origin feature-or-fix-name
```

Example:

```bash
git push origin fix-readme-typo
```

---

## 🔁 Step 8: Create a Pull Request (PR)

1. Go to your fork on GitHub.
2. You’ll see a prompt to create a **Pull Request**.
3. Compare your branch with the **original repo’s** `main` branch.
4. Write a clear PR title and description.
5. Submit your PR 🚀

---

## 🔄 Step 9: Keep Your Fork Updated (Optional but Recommended)

Fetch and merge the latest changes from the original repo:

```bash
git fetch upstream
git merge upstream/main
```

Or rebase (optional advanced method):

```bash
git fetch upstream
git rebase upstream/main
```

---

## ✅ Summary

| Action           | Repository                            |
| ---------------- | ------------------------------------- |
| **Fork**         | Original repo (creates your own copy) |
| **Clone**        | Your fork (to your local machine)     |
| **Push**         | To your fork                          |
| **Pull Request** | From your fork → to the original repo |

---

### 🧠 Tips

* Always read the **`CONTRIBUTING.md`** file in the project before starting.
* Use **meaningful branch names** (e.g., `add-login-feature`, `fix-navbar-bug`).
* Keep your commits small and focused.
* Be polite and open to feedback in PR reviews.

---

### 💖 Happy Contributing!

> “The best way to learn Git and GitHub is by contributing to open source.”
> — You, after your first PR 🎉

