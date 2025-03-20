# This is your introduction page

**Do not rename this file. It is index.md and mkdocs-material looks for it to build the Homepage**

**This list is not in order**

- Add purpose of software
- Add purpose of your specific instruction pages
- Add intended user and level of user: terms like beginner or intermediate are vague: what can a beginner do? What can an intermdiate do and what do they already know?
- Add admonitions and show what they will be used for
- Add conventions: **bold** is for actions, for example
- add prerequisities; "you should already have x installed"

To set up correct navigation order for your published site, make changes in mkdocs.yml, like this: 

nav:
  - Home: "index.md"
  - First page: "Set-1.md"
  - Second page: "Set2.md"
  - Third page: "Set3.md"
  - Troubleshooting: "Troubleshooting.md"
  - Glossary: "Glossary.md"