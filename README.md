# d10-starter
Drupal 10 starter for new projects, attentions this is an opinionated starter.

## Handbook D9/D10
[https://selwynpolit.github.io/d9book/](https://selwynpolit.github.io/d9book/)

## TODOs

- [ ] Check defaults modules  
- [ ] ... 

## What defaults do/active
* Disable users registrations
* Default url paths for content: [node:content-type]/[node:title]

## First commands
```bash
lando drush site:install --db-url=mysql://drupal10:drupal10@database/drupal10 -y
```

### Fix permission
```bash
$ cd /var/www/example.org/public_html/web
$ chown -R johndoe:www-data .
$ find . -type d -exec chmod u=rwx,g=rx,o= '{}' \;
$ find . -type f -exec chmod u=rw,g=r,o= '{}' \;
```

## VSCode configurations
Based on Drupal.org's guide [Configuring Visual Studio Code](https://www.drupal.org/docs/develop/development-tools/editors-and-ides/configuring-visual-studio-code)
### Extensions
* [PHP Sniffer & Beautifier: Combines both phpcs and phpcbf in one handy extension.](https://marketplace.visualstudio.com/items?itemName=ValeryanM.vscode-phpsab&ssr=false#overview)
* [PHP DocBlocker: Provides auto-complete for PHP docblocks.](https://marketplace.visualstudio.com/items?itemName=neilbrayfield.php-docblocker)
* [Empty Indent: Removes indent of empty lines on save.](https://marketplace.visualstudio.com/items?itemName=DmitryDorofeev.empty-indent)
* [PHP Debug: Provides launch configuration support for XDebug. Requires XDebug.](https://marketplace.visualstudio.com/items?itemName=felixfbecker.php-debug)
