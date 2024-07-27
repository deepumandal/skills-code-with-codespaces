<header>

<!--
  <<< Author notes: Course header >>>
  Read <https://skills.github.com/quickstart> for more information about how to build courses using this template.
  Include a 1280×640 image, course name in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280×640 social image, auto delete head branches.
  Next to "About", add description & tags; disable releases, packages, & environments.
  Add your open source license, GitHub uses the MIT license.
-->

# Code with GitHub Codespaces and Visual Studio Code

_Develop code using GitHub Codespaces and Visual Studio Code!_

</header>

<!--
  <<< Author notes: Step 2 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->

## Step 2: Add a custom image to your codespace!

_Nice work! :tada: You created your first codespace and pushed code using VS Code!_

You can configure the development container for a repository so that any codespace created for that repository will give you a tailored development environment, complete with all the tools and runtimes you need to work on a specific project.

**What are development containers?** Development containers, or dev containers, are Docker containers that are specifically configured to provide a fully featured development environment. Whenever you work in a codespace, you are using a dev container on a virtual machine.

A dev container file is a JSON file that lets you customize the default image that runs your codespace, VS code settings, run custom code, forward ports and much more!

Let's add a `devcontainer.json` file and add a custom image.

### :keyboard: Activity: Add a .devcontainer.json file to customize your codespace

1. Navigating back to your **Code** tab of your repository, click the **Add file** drop-down button, and then click `Create new file`.
1. Type or paste the following in the empty text field prompt to name your file.

   ```
   .devcontainer/devcontainer.json
   ```

1. In the body of the new **.devcontainer/devcontainer.json** file, add the following content:

   ```jsonc
   {
     // Name this configuration
     "name": "Codespace for Skills!",
     // Use the base codespace image
     "image": "mcr.microsoft.com/vscode/devcontainers/universal:latest",

     "remoteUser": "codespace",
     "overrideCommand": false
   }
   ```

1. Click **Commit changes** and then select **Commit changes directly to the `main` branch**.
1. Create a new codespace by navigating back to the **Code** tab of your repository.
1. Click the green **Code** button located in the middle of the page.
1. Click the **Codespaces** tab on the box that pops up.
1. Click the **Create codespace on main** button OR click the `+` sign on the tab. This will create a new codespace on the main branch. (Notice your other codespace listed here.)

   > Wait about **2 minutes** for the codespace to spin itself up.

1. Verify that your new codespace is is running, as you did previously.

   Note the image being used is the default image provided for GitHub Codespaces. It includes runtimes and tools for Python, Node.js, Docker, and more. See the full list here: https://aka.ms/ghcs-default-image. Your development team can use any custom image that has the necessary prerequisites installed. For more information, see [codespace image](https://aka.ms/configure-codespace).

1. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.

<footer>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

---

Get help: [Post in our discussion board](https://github.com/orgs/skills/discussions/categories/code-with-codespaces) &bull; [Review the GitHub status page](https://www.githubstatus.com/)

&copy; 2023 GitHub &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT License](https://gh.io/mit)

</footer>
