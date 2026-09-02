# Blog Instructions

## Students READTHIS

### Part 1: Clone the Repo

You do not need to Fork this repository before cloning it.


[VSCode Source Control](https://code.visualstudio.com/docs/sourcecontrol/overview)

[Github Desktop](https://docs.github.com/en/desktop/making-changes-in-a-branch/managing-branches-in-github-desktop)

[Git CLI]()

### Part 2: Add Content

1. In the src/docs/Blog/20XX/ folder, 20XX should match the year you joined CodeSchool, add a folder with your github username on it. 

2. In the folder that you created for your username:

- Create a single file titled `index.md`, `source.md` or `README.md` This file will serve as the home page for your personal section of the blog website.

- The file name for this first file (either `index.md`, `source.md` , or `README.md`) is case sensitive and must be written exactly as displayed here.

- Every folder you create in this repo will need to have one of these files

3. To add more blog posts. Continue creating files in the folder you created with your username. 

When you create new files or folders, do not include spaces or special characters in the file or folder name. Instead use hyphens, underscores, camelCasing, or PascalCasing to indicate multiple words.

Example:
`Code School.md` is an invalid file or folder name because it has a space. ❌
`Code @School#00` is also an invalid file or folder name. ❌

`codeSchool.md`, `CodeSchool.md`, `Code-School.md`, and `Code_School.md` are all valid patterns. ✅


Since Your first blog post will be about a Growth Mindset,
here are some ideas for file names:
```
    GrowthMindset.md
    1-GrowthMindset.md
    08-25-2026.md
```

These are all reasonable choices based on the content, the fact that this is your 1st blog, and that the class is from Aug 25, 2026.

Feel free to be creative and remember to avoid using spaces in the file & folder names.
<!-- folder titled Portfolio with a file that has the same name. -->

![Example File Structre](/Imgs/Blog_File_Structure.png  "image_tooltip")

When your file is added into the repo and live on the site, you will see the title element from your page set as the title in the left nav bar.

In VSCode/Filesystem:
![VSCode's Display of the File Structre](/Imgs/Blog_File_Structure2.png  "image_tooltip")

In a Web Browser:

![Browser Rendered Directory Listing](/Imgs/Blog_File_Structure3.png "image_tooltip")

### Part 3: Update YOUR Link

Now that your content is created in the repo, go back to the `index.md` file in the 2026 folder.

![Site Index File View](/Imgs/Site_Index.png "image_tooltip")

You should see your name alongside a link that is almost pointing to where your blog content sits. 
After the last slash, add your Github username to the link and save the file.

### Git Push, Toast 🍻🥂

Now, simply Add-Commit-Push

[VSCode Source Control](https://code.visualstudio.com/docs/sourcecontrol/overview)

[Github Desktop](https://docs.github.com/en/desktop/making-changes-in-a-branch/managing-branches-in-github-desktop)

Git CLI [A](https://git-scm.com/docs/git-add)-[C](https://git-scm.com/docs/git-commit)-[P](https://git-scm.com/docs/git-push)

`git add -A` <!--add/stage all new and changed files to your next commit-->

`git commit -m "mrjones91 blog and directions"` <!-- create your commit and set a custom message to log what contents are in this update -->

`git push` <!-- push your changes back to the repo--> 

If your `git push` command fails, try using `git pull`.

 `git pull` <!-- Will update your local repository with the changes from the cloud. -->

Then try to `git push` again.
