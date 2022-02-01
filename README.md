# tex templates
Personal LaTeX document class files. 

## Usage
The easiest way to use this template is to have Github use this template and create a repository for you. 

However, the template can get out of date (since it is a WIP). To handle updates more easily, it might be beneficial to create repositories that are forks instead of template derivatives. I'm still figuring it out but it might be beneficial to have this repository (tex-template) as a submodule. 

For now, you can add this template as a remote: 
```
git remote add template git@github.com:jchen/tex-template.git
```
Then fetch this remote (along with your current remote)
```
git fetch --all
```
and finally do a 'hard merge' from the template
```
git merge template/main --allow-unrelated-histories
```

If merge conflicts arise, the class file can be manually resolved through
```
git checkout --theirs jiahua.cls
git add jiahua.cls
```
and
```
git checkout --ours [file]
git add [file]
```
for any other merge conflicts to keep the new changes. 
