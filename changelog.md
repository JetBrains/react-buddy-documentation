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


## 2022.5 (2022-10-19)

### Features
* Component tree view in the Project tool window
  * Displays hierarchy of React application components
  * Displays paths of components used in routing (supporting react-router)
* Quick fix to add new props to a component straight from JSX
* Intention to wrap a functional component to `React.memo()`
* Now it's possible to configure the type of generated handlers (function declaration/function expression)
* Gutter icons provided by the plugin are now configurable (you can switch off unnecessary icons in IDE's settings)
* Hooks-related features are now available only if project's React supports hooks (16.8+)

Number of performance improvements and bugfixes

## 2022.4 (2022-08-15)

### Features
* Code preview for the palette components and code generation actions
* An action to create a new React component from project tree
* Complex palette snippets (defined as prototypes) now support passing local variables as parameters
* `useRef` generation intention
* Built-in React hooks are added to the palette
* JSX Outline now supports arrays of JSX elements
* Components from palette now can be added to an arbitrary part of the component (npt only inside the JSX)

Number of performance improvements and bugfixes

