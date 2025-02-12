# Mise and DirenV
------------------------------------------------

## Mise
Mise is a handy terminal tool, which helps me to always install the version of java, etc. I wants.

### Tutorial
1. Go to the file mise.toml
2. Define in the file what I want to install and which version
3. For example: java = 'openjdk-17.0.2'
4. Go to the terminal and type in "mise install"
5. Now it installed everything I defined in that file

### Other commands
- "mise plugins ls-remote" = shows list of all options to install
- "mise ls-remote java" = shows all available version of for example java
- Example: "mise ls-remote java" = all java versions you can install

## DirenV
Direnv is a terminal tool that automatically loads / unloads environment variables based on the directory I'm in.

### Tutorial
1. Create a ".envrc" file (never commit this file for safety reasons)
2. Define everything in there like keys, etc.
3. Example: export TEST_TOKEN=Token_test123456
4. Go to the terminal and type in "direnv allow"
5. Now everything is updated

----------------------------
### Other useful commands
- To build: "npx nx run “name”:build" —> building what I wanted to be built