https://davidwalsh.name/convert-websites-apps

npm install nativefier # App creator
npm install node-icns  # Icon creator

# Generate icon set required by macOS
node_modules/.bin/nicns --in app-icon.png --out app-icon.icns

node_modules/.bin/nativefier \
    --name "David Walsh Blog" \
    --verbose \
    --counter \
    --icon app-icons.icns \
    --fast-quit \
    --inject custom-css.css \
    --inject custom-js.js \
    --flash # gross
    "https://davidwalsh.name"

Conf parameters manual: https://github.com/jiahaog/nativefier/blob/development/docs/api.md

# Workplace
node_modules/.bin/nativefier --name 'Workplace' --verbose --counter --icon img/workplace.icns --fast-quit "https://www.facebook.com/workplace"
node_modules/.bin/nativefier --name 'Workplace' --verbose --counter --icon img/workplace.icns --fast-quit "https://work-66665164.facebook.com"

# Work Chat
node_modules/.bin/nativefier --name 'Work Chat' --verbose --counter --icon img/workplace.icns --fast-quit "https://work-66665164.facebook.com/chat/"

# Trello
node_modules/.bin/nativefier --name Trello --verbose --counter --icon trello-app-icon.icns --fast-quit --maximize --disable-dev-tools "https://trello.com"
