# [Itellij Plugin](https://plugins.jetbrains.com/plugin/17467-react-buddy/) Changelog

## 2023.1 (2023-02-17)

### Breaking changes
We fixed an issue with the plugin settings synchronisation. Please reapply global settings in Preferences -> React Buddy.

### Features
* Storybook support
  * Storybook components tool window (displays stories defined inside the project)
  * Code generation by Storybook stories (d'n'd from the tool window / use code generation action)
  * Intention for adding components to Storybook
  * Note: MDX format currently is not supported
* Coding assistance for state generation
  * Intention to convert local variable to useState
  * Quick-fix to create state variable from non-existing symbol passed to a JSX prop
  * `.state` postfix completion
* Conditional rendering support
  *Intention to wrap JSX element into condition
  * Live template for `wrap into` action
  * Action in the JSX Outline
* Ant Design support
  * Visual designer for Antd Form.Item validation rules

### Improvements
* Palette matching mechanism become more [transparent](https://github.com/react-buddy/palettes/blob/main/palettes.json)
* Improved punctuation support (respect semicolon setting in IDE)
* Better component preview line marker placement

Number of performance improvements and bugfixes