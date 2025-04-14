# Hi there, I'm Tadese Ayane 👋

Welcome to my GitHub profile! I'm a passionate developer with a keen interest in solving real-world problems with clean, efficient, and innovative code. I thrive on learning new technologies and collaborating on exciting projects.

---

## 🌟 About Me

- 🔭 I’m currently working on **[Your Current Project/Interest]**.
- 🌱 I’m learning **[Technologies or Skills You're Learning]**.
- 💡 I enjoy contributing to open source and exploring **[Your Area of Interest]**.
- 💬 Ask me about **[Your Expertise or Favorite Topics]**.
- 📫 How to reach me: [Your Contact Information or Links].
- ⚡ Fun fact: **[Something Fun About You]**.

---

## 🛠️ Technologies & Tools

- **Languages:** [Add your most-used languages, e.g., Python, JavaScript, etc.]
- **Frameworks & Libraries:** [Add relevant ones, e.g., React, Django, etc.]
- **Tools:** [Add tools, e.g., Docker, Git, etc.]
- **Other Skills:** [Any other skill worth mentioning].

---

## 📈 GitHub Stats

![Tadese's GitHub Stats](https://github-readme-stats.vercel.app/api?username=tadese-ayane&show_icons=true&theme=radical)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=tadese-ayane&layout=compact&theme=radical)

---

## 🚀 Let's Connect

- 💼 [LinkedIn](#)
- 🐦 [Twitter](#)
- 🌐 [Personal Website/Portfolio](#)
- 📧 [Email](mailto:#)

---

✨ **"Code is like humor. When you have to explain it, it’s bad." – Cory House** ✨
name: Step 1, Enable GitHub Pages

# This step triggers after we run a pages build.
# This workflow updates from step 1 to step 2.

# This will run every time we run a pages build.
# Reference: https://docs.github.com/en/actions/learn-github-actions/events-that-trigger-workflows
on:
  workflow_dispatch:
  page_build:

# Reference: https://docs.github.com/en/actions/security-guides/automatic-token-authentication
permissions:
  # Need `contents: read` to checkout the repository.
  # Need `contents: write` to update the step metadata.
  contents: write

jobs:
  # Get the current step to only run the main job when the learner is on the same step.
  get_current_step:
    name: Check current step number
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v4
      - id: get_step
        run: |
          echo "current_step=$(cat ./.github/steps/-step.txt)" >> $GITHUB_OUTPUT
    outputs:
      current_step: ${{ steps.get_step.outputs.current_step }}

  on_enable_github_pages:
    name: On enable github pages
    needs: get_current_step

    # We will only run this action when:
# 1. This repository isn't the template repository.
# 2. The step is currently 1.
# Reference: https://docs.github.com/en/actions/learn-github-actions/contexts
# Reference: https://docs.github.com/en/actions/learn-github-actions/expressions
if: >-
  ${{ !github.event.repository.is_template
      && needs.get_current_step.outputs.current_step == 1 }}

# We'll run Ubuntu for performance instead of Mac or Windows.
runs-on: ubuntu-latest

steps:
  # We'll need to check out the repository so that we can edit the README.
  - name: Checkout
    uses: actions/checkout@v4
    with:
      fetch-depth: 0 # Let's get all the branches.
      ref: my-pages

  # In README.md, switch step 1 for step 2.
  - name: Update to step 2
    uses: skills/action-update-step@v2
    with:
      token: ${{ secrets.GITHUB_TOKEN }}
      from_step: 1
      to_step: 2
      branch_name: my-pages
