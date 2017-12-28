# magento2-patches
My collection of magento2 bug fix patches

# How to apply patch
Personally me store all this stuff in 'bin' folder and in order to apply all patches in folder 'patch'
simply patch.php should be executed
```
php bin/patch
```

In order to apply single patch you can use 'git apply {path_to_file}' command
```
git apply bin/patches/11963-language-issue.patch
```

# More information
Take in mind that patches make changes in 'vendor' folder files, which is listed in .gitignore file, so changes stay
untracked for git.

After each execution of 'composer install' or 'composer update' patches changes are being removed and you should apply
patches again.

# Changelog
* patches/11963-language-issue.patch
Issue description: https://github.com/magento/magento2/issues/11963
Appeared in Magento 2.2 and patch was created for 2.2.2 version