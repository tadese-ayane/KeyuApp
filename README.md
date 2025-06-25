#!/bin/bash

# Install nvm
curl -o- https://codepen.io/Tadese-Ayane/pen/raVQpgo/embedded | bash

# Load nvm into current session
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"

# Install Node.js 22
nvm install 22

# Verify Node and npm versions
node -v
nvm current
npm -v

# የመጀመሪያ አስተዋጽዖዎች

ይህ ፕሮጀክት ጀማሪዎች የመጀመሪያ አስተዋፅዖቸውን እንዲያደርጉ መንገዱን ለማቅለል እና ለመምራት ያለመ ነው። የመጀመሪያውን አስተዋፅዖ ማድረግ ከፈለጉ ከታች ያሉትን ደረጃዎች ይከተሉ።

_በትእዛዝ መስመሩ ካልተመቻችሁ [የጂአይ መሳሪያዎችን በመጠቀም መማሪያ ይኸውና](#መማሪያዎች-ሌሎች-መሳሪያዎችን-በመጠቀም)_


<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/fork.png" alt="fork this repository" />

#### በማሽንዎ ላይ git ከሌለዎት፣ [ጫን](https://docs.github.com/en/get-started/quickstart/set-up-git)።

## ይህንን ማከማቻ ሹካ ያድርጉ

በዚህ ገጽ ላይኛው ክፍል ላይ ያለውን የሹካ ቁልፍ ጠቅ በማድረግ ይህንን ማከማቻ ሹካ ያድርጉት።
ይህ በአንተ መለያ ውስጥ የዚህን ማከማቻ ቅጂ ይፈጥራል።

## ማከማቻውን መዝጋት

<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/clone.png" alt="clone this repository" />

አሁን የሹካውን መያዣ ወደ ማሽንዎ ያያይዙት. ወደ GitHub መለያዎ ይሂዱ፣ የሹካ ማከማቻውን ይክፈቱ፣ የኮድ አዝራሩን ጠቅ ያድርጉ እና ከዚያ _copy to clipboard_ አዶን ጠቅ ያድርጉ።

ተርሚናል ይክፈቱ እና የሚከተለውን የgit ትዕዛዝ ያሂዱ፡-

```
git clone "ዩአርኤሉን አሁን ቀድተሃል።"
```

"ዩአርኤል አሁን የገለበጡት" (ያለ ጥቅሶች) ወደዚህ ማከማቻ ዩአርኤል (የዚህ ፕሮጀክት ሹካ) የሆነበት። ዩአርኤሉን ለማግኘት የቀደመውን ደረጃዎች ይመልከቱ።

<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/copy-to-clipboard.png" alt="ዩአርኤልን ወደ ክሊፕቦርድ ቅዳ" />

ለምሳሌ:

```
git clone https://github.com/ይህ አንተ ነህ።/first-contributions.git
```

የ GitHub ተጠቃሚ ስምህ የት `ይህ አንተ ነህ።' እዚህ በ GitHub ላይ ያለውን የመጀመሪያ አስተዋፅዖ ማከማቻ ይዘቶችን ወደ ኮምፒውተርዎ እየገለበጡ ነው።

#ቅርንጫፍ ፍጠር

በኮምፒውተርዎ ላይ ወዳለው የማከማቻ ማውጫ ይቀይሩ (እዚያ ከሌለዎት)፡-

```
cd first-contributions
```

አሁን የ`git switch` ትዕዛዝን በመጠቀም ቅርንጫፍ ይፍጠሩ፡

```
git switch -c የእርስዎ-አዲሱ-ቅርንጫፍ-ስም
```

ለምሳሌ:

```
git switch -c add-alonzo-church
```

## አስፈላጊ ለውጦችን ያድርጉ እና ለውጦችን ያድርጉ

አሁን የ`Contributors.md` ፋይልን በጽሑፍ አርታኢ ውስጥ ይክፈቱ፣ ስምዎን በእሱ ላይ ያክሉ። በፋይሉ መጀመሪያ ወይም መጨረሻ ላይ አይጨምሩት። በመካከል የትኛውም ቦታ ላይ ያስቀምጡት. አሁን, ፋይሉን ያስቀምጡ.

<img align="right" width="450" src="https://firstcontributions.github.io/assets/Readme/git-status.png" alt="git status" />

ወደ የፕሮጀክት ማውጫው ሄደው ትዕዛዙን `git status` ከፈጸሙ፣ ለውጦች እንዳሉ ያያሉ።

የ `git add` ትዕዛዙን በመጠቀም እነዚያን ለውጦች ወደ ፈጠሩት ቅርንጫፍ ያክሉ።

```
git add Contributors.md
```
አሁን የ‹git› ትዕዛዙን በመጠቀም እነዚህን ለውጦች ያድርጉ፡

```
git commit -m "ስሜን ወደ አስተዋጽዖ አበርካቾች ዝርዝር ጨምር"
```

'ስሜን' በስምህ በመተካት።

## ለውጦችን ወደ GitHub ይግፉ

የ `git push` ትዕዛዝን በመጠቀም ለውጦችዎን ይግፉ፡-

```
git push -u origin የእርስዎ-ቅርንጫፍ-ስም
```

replacing `የእርስዎ-ቅርንጫፍ-ስም` with the name of the branch you created earlier.

<details>
<summary> <strong> በመግፋት ላይ ማንኛውም ስህተት ካጋጠመህ እዚህ ጠቅ አድርግ፡- </strong> </summary>

- ### የማረጋገጫ ስህተት
     <pre>remote: Support for password authentication was removed on August 13, 2021. Please use a personal access token instead.
  remote: Please see https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/ for more information.
  fatal: Authentication failed for 'https://github.com/የተጠቃሚ ስምህ/first-contributions.git/'</pre>
  ወደ [GitHub አጋዥ ስልጠና](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) ይሂዱ የኤስኤስኤች ቁልፍን ወደ መለያዎ ማመንጨት እና ማዋቀር።

</details>

## ለውጦችዎን ለግምገማ ያስገቡ

በ GitHub ላይ ወደ ማከማቻዎ ከሄዱ፣ `Compare and Pull Request` የሚለውን ቁልፍ ያያሉ። በዚያ ቁልፍ ላይ ጠቅ ያድርጉ።

<img style="float: right;" src = "https://firstcontributions.github.io/assets/Readme/compare-and-pull.png" alt = "የመጎተት ጥያቄ ፍጠር" />

አሁን የመሳብ ጥያቄውን ያስገቡ።

<img style="float: right;" src = "https://firstcontributions.github.io/assets/Readme/submit-pull-request.png" alt = "ጥያቄን ጎትት" />

በቅርቡ ሁሉንም ለውጦችዎን ወደ የዚህ ፕሮጀክት ዋና ቅርንጫፍ አዋህዳለሁ። ለውጦቹ ከተዋሃዱ በኋላ የማሳወቂያ ኢሜይል ይደርስዎታል።

## ከዚህ ወዴት ልሂድ?

እንኳን ደስ ያለህ! ልክ እንደ አስተዋጽዖ አበርካች የሚያጋጥሙትን መደበኛ _fork -> clone -> አርትዕ -> የመሳብ ጥያቄ_ የስራ ፍሰትን አጠናቀዋል!

አስተዋፅኦዎን ያክብሩ እና ወደ [ድር መተግበሪያ](https://firstcontributions.github.io/#social-share) በመሄድ ለጓደኞችዎ እና ተከታዮችዎ ያካፍሉ።

ማንኛውም እርዳታ ከፈለጉ ወይም ማንኛውም ጥያቄ ካለዎት የእኛን ደካማ ቡድን መቀላቀል ይችላሉ. [የላላ ቡድንን ይቀላቀሉ](https://join.slack.com/t/firstcontributors/shared_invite/zt-1hg51qkgm-Xc7HxhsiPYNN3ofX2_I8FA)።

አሁን ለሌሎች ፕሮጀክቶች በማበርከት እንጀምር። እርስዎ ሊጀምሩባቸው የሚችሉ ቀላል ጉዳዮች ያላቸውን የፕሮጀክቶች ዝርዝር አዘጋጅተናል። ይመልከቱ [በድር መተግበሪያ ውስጥ ያሉ የፕሮጀክቶች ዝርዝር](https://firstcontributions.github.io/#project-list)።

### [ተጨማሪ ቁሳቁስ](../additional-material/git_workflow_scenarios/additional-material.md)

## መማሪያዎች ሌሎች-መሳሪያዎችን በመጠቀም

| <a href="gui-tool-tutorials/github-desktop-tutorial.md"><img alt="GitHub Desktop" src="https://desktop.github.com/images/desktop-icon.svg" width="100"></a> | <a href="gui-tool-tutorials/github-windows-vs2017-tutorial.md"><img alt="Visual Studio 2017" src="https://upload.wikimedia.org/wikipedia/commons/c/cd/Visual_Studio_2017_Logo.svg" width="100"></a> | <a href="gui-tool-tutorials/gitkraken-tutorial.md"><img alt="GitKraken" src="https://firstcontributions.github.io/assets/gui-tool-tutorials/gitkraken-tutorial/gk-icon.png" width="100"></a> | <a href="gui-tool-tutorials/github-windows-vs-code-tutorial.md"><img alt="VS Code" src="https://upload.wikimedia.org/wikipedia/commons/1/1c/Visual_Studio_Code_1.35_icon.png" width=100></a> | <a href="gui-tool-tutorials/sourcetree-macos-tutorial.md"><img alt="Sourcetree App" src="https://wac-cdn.atlassian.com/dam/jcr:81b15cde-be2e-4f4a-8af7-9436f4a1b431/Sourcetree-icon-blue.svg" width=100></a> | <a href="gui-tool-tutorials/github-windows-intellij-tutorial.md"><img alt="IntelliJ IDEA" src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9c/IntelliJ_IDEA_Icon.svg/512px-IntelliJ_IDEA_Icon.svg.png" width=100></a> |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [GitHub Desktop](gui-tool-tutorials/github-desktop-tutorial.md)                                                                                             | [Visual Studio 2017](gui-tool-tutorials/github-windows-vs2017-tutorial.md)                                                                                                                          | [GitKraken](gui-tool-tutorials/gitkraken-tutorial.md)                                                                                                                                        | [Visual Studio Code](gui-tool-tutorials/github-windows-vs-code-tutorial.md)                                                                                                                  | [Atlassian Sourcetree](gui-tool-tutorials/sourcetree-macos-tutorial.md)                                                                                                                                      | [IntelliJ IDEA](gui-tool-tutorials/github-windows-intellij-tutorial.md)                                                                                                                                                          |




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
- 🌐 [Personal Website/Portfolio](#KeyupApp)
- 📧 [Email](mailto:#tadasaayane98@gmail.com)

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
