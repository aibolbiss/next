# Как установить NVM?
1) https://github.com/nvm-sh/nvm#install--update-script     -      ссылка для скачивания nvm
2) curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash     -     вставляем в терминал
3) export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm          -       вставляем в терминал
4) nvm --version
5) nvm install 12
6) node -v
7) nvm install 14
8) nvm use 14

# Как установить TypeScript?
1) npm install -g typescript
