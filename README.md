# Nativefier usage examples on macOS

Initially based on https://davidwalsh.name/convert-websites-apps

## Prerequisites
- `npm install nativefier`
- if you want automatic icon conversion to icns then you should have imagemagick (`brew install imagemagick`) and iconutil (comes with Xcode?), otherwise see https://github.com/jiahaog/nativefier/blob/HEAD/docs/api.md#icon for manual conversion options

Conf parameters manual: https://github.com/jiahaog/nativefier/blob/development/docs/api.md

## Usage examples

### Jupyter Notebook
`node_modules/.bin/nativefier --name 'Jupyter Notebook' --verbose --counter --icon img/jupyter.notebook.png --maximize --fast-quit --disable-dev-tools --single-instance "http://localhost:8888/"`

### Workplace
`node_modules/.bin/nativefier --name 'Workplace' --verbose --counter --icon img/workplace.icns --fast-quit --disable-dev-tools --single-instance "https://work-66665164.facebook.com"`

### Work Chat
`node_modules/.bin/nativefier --name 'Work Chat' --verbose --counter --icon img/workplace.icns --fast-quit "https://work-66665164.facebook.com/chat/"`

### Trello
`node_modules/.bin/nativefier --name Trello --verbose --counter --icon img/trello-app-icon.icns --fast-quit --maximize --disable-dev-tools "https://trello.com"`

### GitHub
`node_modules/.bin/nativefier --name GitHub --verbose --counter --icon img/github.icns --fast-quit --maximize --disable-dev-tools -e 1.7.5 --single-instance "https://github.com"`
