# [Intellij Plugin](https://plugins.jetbrains.com/plugin/17467-react-buddy/) Changelog

## 2023.2.4 (2023-06-23)

This release contains version compatible with latest EAP as well as number of stability improvements and fixes

[All resolved issues](https://issues.react-buddy.com/issues/RCB?q=Milestone:%2023.2.4)

## 2023.2.3 (2023-06-07)

This release contains bugfixes and stability improvements

[All resolved issues](https://issues.react-buddy.com/issues/RCB?q=Milestone:%2023.2.3)

## 2023.2.2 (2023-05-25)

* The version compatible with IntelliJ 23.2 EAP has been published.
* In a newly opened project React Buddy's tool-windows expanded only if `palette.tsx` defined.
* A number of bugfixes and improvements.

[All resolved issues](https://issues.react-buddy.com/issues/RCB?q=Milestone:%2023.2.2)

## 2023.2.1 (2023-05-11)

### Improvements

* New prop generation: added heuristics to avoid collisions with existing props [RCB-779](https://issues.react-buddy.com/issue/RCB-779)
* Now the plugin is being activated even if React is added as a transitive dependency [RCB-793](https://issues.react-buddy.com/issue/RCB-793)
* Create a new React component action: the most recently selected component type is used by default [RCB-798](https://issues.react-buddy.com/issue/RCB-798)

### Fixes

* The annoying `Synchronous execution under ReadAction` exception and number of other minor issues are fixed

[All resolved issues](https://issues.react-buddy.com/issues/RCB?q=Milestone:%2023.2.1)

## 2023.2 (2023-05-02)

### Features
* Quick-fix for adding new props to a current React component (from unresolved symbol or empty prop in JSX) [683](https://issues.react-buddy.com/issue/RCB-683) [RCB-764](https://issues.react-buddy.com/issue/RCB-764)
* Most elements in base React palette are now editable live templates [RCB-755](https://issues.react-buddy.com/issue/RCB-755)
* New live templates and palette elements for React components creation [RCB-682](https://issues.react-buddy.com/issue/RCB-682)
* New live template for context generation: `ctx` [RCB-673](https://issues.react-buddy.com/issue/RCB-673/React-context-code-generation)
* Storybook
  * CSF 3 (Storybook 7) support [RCB-691](https://issues.react-buddy.com/issue/RCB-691)
  * Storybook category in React Palette [RCB-746](https://issues.react-buddy.com/issue/RCB-746)
  * Drag and Drop from Storybook tool-window to the JSX Outline [RCB-745](https://issues.react-buddy.com/issue/RCB-745)
  * Project tree action for new `.stories` file creation [RCB-747](https://issues.react-buddy.com/issue/RCB-747)

### Improvements
* Auto-import improvements [RCB-742](https://issues.react-buddy.com/issue/RCB-742)
* Better JS keywords treatment on code generation [RCB-723](https://issues.react-buddy.com/issue/RCB-723)

[All resolved issues](https://issues.react-buddy.com/issues/RCB?q=Milestone:%2023.2)

## 2023.1.5 (2023-04-21)
* Fixed FilenameIndex exception on project open [RCB-778](https://issues.react-buddy.com/issue/RCB-778/comintellijpsisearchFilenameIndex-throw-javalangThrowable-Assertion-failed)
* Images were revomed from the plugin description.

## 2023.1.4 (2023-04-18)
* React 18 support (added new hooks), updated doc links to react.dev
* WSL 2 support [RCB-768](https://issues.react-buddy.com/issue/RCB-768/Issue-with-project-placed-in-WSL-2)

[All resolved issues](https://issues.react-buddy.com/issues/RCB?q=Milestone:%2023.1.4)

## 2023.1.3 (2023-04-04)
* Fixed back and forward navigation in tsx/jsx files [RCB-758](https://issues.react-buddy.com/issue/RCB-758/Back-and-forward-navigation-is-broken-in-tsxjsx-files)
* Categories in the Storybook tool-window are sorted alphabetically. Stories are sorted in definition order. [RCB-736](https://issues.react-buddy.com/issue/RCB-736/Sort-storybook-categories-alphabetically-stories-in-definition-order)
* Upgrade Mantine installation logic to use v6 [RCB-740](https://issues.react-buddy.com/issue/RCB-740/Upgrade-Install-React-Library-UI-kit-version-for-Mantine)
* Fix JSX map inspection for IntelliJ 2023.1 [RCB-733](https://issues.react-buddy.com/issue/RCB-733/The-231-version-of-intellIJ-IDEA-has-no-JSX-map-inspection)

[All resolved issues](https://issues.react-buddy.com/issues/RCB?q=Milestone:%2023.1.3)

## 2023.1.2 (2023-03-15)
* Next.js support - component preview now works in projects based on Next.js@10+ with experimental `@react-buddy/ide-toolbox-next`. [RCB-353](https://issues.react-buddy.com/issue/RCB-353)
* Preview initialisation improvements [RCB-704](https://issues.react-buddy.com/issue/RCB-704/IDE-closes-itself-when-changing-dev-server-port-number)

[All resolved issues](https://issues.react-buddy.com/issues/RCB?q=Milestone:%2023.1.2)

## 2023.1.1 (2023-03-02)
* Support for TypeScript path aliases [RCB-687](https://issues.react-buddy.com/issue/RCB-687)
* React Buddy now respects IDE semicolon settings for TypeScript and JavaScript [RCB-688](https://issues.react-buddy.com/issue/RCB-688)
* Navigation to a particular Storybook story from the tool window [RCB-697](https://issues.react-buddy.com/issue/RCB-697)
* Version adapted to IJ 2023.1 Beta
* Improved preact support

[All resolved issues](https://issues.react-buddy.com/issues/RCB?q=Milestone:%2023.1.1)

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
* Quick fix to add missing deps to `useCallback()` and `useMemo()`. Automatically deactivates if eslint integration is on.
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

## 2022.3 (2022-06-27)

### Features
* Ability to add a popular UI library to a project Currently, it's in incubator stage and is available through the find action menu (ctrl/cmd + a). Type `Install React Library` to find the action
  * Ant.Design
  * MUI
  * ChakraUI
  * Mantine
  * NativeBase
  * NextUI
* Live templates for React hooks:
  * `usest` - useState
  * `usee` - useEffect
  * `usec` - useContext
  * `userd` - useReducer
  * `usecb` - useCallback
  * `usem` - useMemo
  * `user` - useRef
  * `useih` - useImperativeHandle
  * `usele` - useLayoutEffect
  * `usedv` - useDebugValue
* Improved preview dev server configuration - now we detect the port of the dev server automatically
* Also, the plugin detects if some library in a project has an existing palette and offers to install one as an npm dependency
* Documentation URL now can be specified for each palette component and variant. To open the documentation use the corresponding icon on the top bar.
* Now the Outline allows to move JSX between different components

## 2022.2 (2022-04-27)

In this release we were focused on two features: advanced code generation and component metadata protocol. Both features are in the Incubator. It means they are in the active development phase, with major improvements and changes planned in the nearest future.

* The Metadata protocol allows to:
  * Specify component props used to distinguish elements in the Outline
  * Customize groups and props ordering in the Inspector
* Advanced code generation mechanism with the following features for snippets:
  * Can be declared in a separate files (prototypes).
  * Now may contain hooks and event handlers.
  * Parametrization support
* Added an ability to declare sub-components in the Palette.

Usability improvements and bugfixes.

## 2022.1 (2022-03-16)

The first stable release! Among features and significant improvements, the cardinal change is the preview which works on arbitrary projects (no need to use `@react-buddy/react-scripts` anymore). Other changes are listed below:

* Support projects on pure JavaScript. Previously only TypeScript-based projects were supported.
* Support workspaces with several apps
* Automated setup of `@react-buddy/ide-toolbox`. The plugin will offer to add the dependency and all required files (palette/preview).
* React hook code generation action.
* Batch palette creation mechanism.
* Ability to search and copy/paste nodes in the JSX Outline.
* Handlers and other local functions are now displayed in the JSX Outline.
* Gutter icons for handlers in code editor.
* Antd and MUI palettes were published as npm packages.
* Palettes can be added as dependencies.

Bugfixes and improvements.
