# Nativefier usage examples

Based on https://davidwalsh.name/convert-websites-apps

## Prerequisites
- `npm install nativefier`
- `npm install node-icns`

## Generate icon set required by macOS
- `node_modules/.bin/nicns --in app-icon.png --out app-icon.icns`

Conf parameters manual: https://github.com/jiahaog/nativefier/blob/development/docs/api.md

### Workplace
node_modules/.bin/nativefier --name 'Workplace' --verbose --counter --icon img/workplace.icns --fast-quit --disable-dev-tools --single-instance "https://work-66665164.facebook.com"

### Work Chat
node_modules/.bin/nativefier --name 'Work Chat' --verbose --counter --icon img/workplace.icns --fast-quit "https://work-66665164.facebook.com/chat/"

### Trello
node_modules/.bin/nativefier --name Trello --verbose --counter --icon img/trello-app-icon.icns --fast-quit --maximize --disable-dev-tools "https://trello.com"

### GitHub
node_modules/.bin/nativefier --name GitHub --verbose --counter --icon img/github.icns --fast-quit --maximize --disable-dev-tools -e 1.7.5 --single-instance "https://github.com"
