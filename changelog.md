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


## 2022.6 (2022-12-22)

### Features
* Preview
  * Ability to see component re-renders
  * Now the preview is refreshed by default. Re-initialization is moved to a separate action.
  * Action to navigate to the preview registration
* Preview of palette components is now also available in code generation dialog
* Intention to wrap an event handler in `useCallback()`
* Quick fix to add missing deps `touseCallback()` and `useMemo()` Automatically deactivates if eslint integration is on
* JSX outline
  * An appearance of the outline can be stored and applied for new editors (see the plugin settings)
  * Action to insert a component form the palette
  * Hooks visibility control
  * Ability to reorder components in a file
* Basic preact support (preview and library installation currently does not work)
* `useRef` now is being generated with nullable type

### Incubator Features
* App templates
  * Form designer
  * Card list designer

Number of performance improvements and bugfixes

