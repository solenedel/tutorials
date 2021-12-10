# Setting up AirBNB linter in a project with ESlint

## [tutorial link](https://www.youtube.com/watch?v=SydnKbGc7W8)

1. In VScode, download the ESlint extension, and the Prettier extension.
2. Add global settings: `control + ,` search `format on save` and make sure the User setting is checked.  
3. Search for Prettier and the global (User setting) 
4. In the project directory, run the command: 
   `npm i -D eslint prettier eslint-plugin-prettier eslint-config-prettier eslint-plugin-node eslint-config-node`
   
5. Run this command: `npx install-peerdeps --dev eslint-config-airbnb`
6. In the main project folder, create the file: `.prettierrc` and add any desired rules (must be in JSON format).
7. Run `sudo npm i -g eslint` and then `eslint --init` then answer the questions (can be changed in the file later).
8. 
9. 
10. 

