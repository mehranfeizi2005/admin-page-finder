admin page finder
A script to find admin login pages and EAR vulnerabilites.

#### Features
- [x] Multi-threading on demand
- [x] Big path list (482 paths)
- [x] Supports php, asp and html extensions
- [x] Checks for potential EAR vulnerabilites
- [x] Checks for robots.txt
- [x] Support for custom patns

### Usages
- Check all paths with php extension
```
python adminpagefinder.py -u example.com --type php
```
- Check all paths with php extension with threads
```
python adminpagefinder.py -u example.com --type php --fast
```
- Check all paths without threads
```
python adminpagefinder.py -u example.com
```
- Adding a custom path. For example if you want all paths to start with /data (example.com/data/...) you can do this:
```
python adminpagefinder.py -u example.com --path /data
```
<b>Note: </b> When you specify an extension using <b>--type</b> option, adminpagefinder.py includes paths of that extension as well as paths with no extensions like <b>/admin/login</b>
