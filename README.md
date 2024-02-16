<h1 align="center">Laraphense</h1>

Laraphense is code intelligence for productive [Laravel](https://laravel.com/) development.

# Features

-   [Show Suggestions based on the Laravel version](#show-suggestions-based-on-the-laravel-version)
-   [Auto-Completion](#auto-completion)
-   [Files Creation](#files-creation)
-   [Go to View](#go-to-view)
-   [Env File Syntax Highlighting](#env-file-syntax-highlighting)
-   [Curly Braces Spacer](#curly-braces-spacer)

## Requirements

You Must have a workspace open having Laravel Installed.

### Show Suggestions based on the Laravel version

-   [Version History of Blade Directives](https://github.com/porifa/vscode-laraphense/blob/main/docs/BladeDirectives.md)
-   [Version History of Validation Rules](https://github.com/porifa/vscode-laraphense/blob/main/docs/ValidationRules.md)

### Auto-Completion

-   Suggests Blade Directives
-   Suggests Route names and route parameters
-   Suggests Views and variables
-   Suggests Configs keys
-   Suggests Translations and translation parameters
-   Suggests Laravel mix function
-   Suggests Validation rules
-   Suggests View sections and stacks
-   Suggests Env Variables
-   Suggests Route Middlewares
-   Suggests Asset in the public directory

### Files Creation

-   Create View (Blade) Files by selecting a valid string
-   Auto Suggest creating a view file if already doesn't exist

### Go To View

-   Go to view from blade and PHP files

### Env File Syntax Highlighting

-   Syntax Highlighting for environment files like (.env, .env.example)

### Curly Braces/brackets Spacer

-   Add Spaces between curly braces

## Extension Settings

These are the setting you can use.

### Customize the Maximum number of scanning rows

```json
"Laraphense.maxLinesCount": 1000
```

default is 1000.

### Add Custom Validation Rules as an object

```json
"Laraphense.customValidationRules": {}
```

for validation rule auto-completion.

### Add Models path as an array

```json
"Laraphense.modelsPaths": ["app", "app/Models" ]
```

these 2 paths are included by default

### Customize view file extensions

```json
"Laraphense.viewExtensions": [".blade.php", ".vue" ]
```

these 2 extensions are included by default

### Customize view folders paths

```json
"Laraphense.viewFolders": {
                            "default": "/resources/views",
                            "js": "/resources/js/Pages",
                            "livewire": "/resources/views/livewire",
                            "vendor": "/resources/views/vendor"
                        }
```

these 3 extensions are included by default,

### Add View Directory Separator

```json
"Laraphense.viewDirectorySeparator": "."
```

default is ".", you can use "/".

### Enable/Disable creating a view file from any valid string

```json
"Laraphense.createViewEveryWhere": true
```

to enable or disable creating a view file from EveryWhere.

### Enable/Disable Go To View

```json
"Laraphense.disableGoToView": false
```

If you want to disable the go-to view feature, set this to true.

### Enable/Disable Go To Config

```json
"Laraphense.disableGoToConfig": false
```

If you want to disable the go-to config feature, set this to true.

### Enable/Disable Assets Auto-Completion

```json
"Laraphense.disableAssetCompletion": false
```

If you want to disable assets autocomplete set this to true.

### Enable/Disable Auth Auto-Completion

```json
"Laraphense.disableAuthCompletion": false
```

If you want to disable auth autocomplete set this to true.

### Enable/Disable Blade Auto-Completion

```json
"Laraphense.disableBladeCompletion": false
```

If you want to disable blade directives autocomplete set this to true.

### Enable/Disable Controller Auto-Completion

```json
"Laraphense.disableControllerCompletion": false
```

If you want to disable Controller autocomplete set this to true.

### Enable/Disable Config Auto-Completion

```json
"Laraphense.disableConfigCompletion": false
```

If you want to disable config autocomplete set this to true.

### Enable/Disable Curly Braces Spacer

```json
"Laraphense.disableCurlyBracesSpacer": false
```

to enable or disable Curly Braces Spacer. By default, it is enabled

### Enable/Disable Eloquent Auto-Completion

```json
"Laraphense.disableEloquentCompletion": false
```

If you want to disable Eloquent autocomplete set this to true.

### Enable/Disable Env Auto-Completion

```json
"Laraphense.disableEnvCompletion": false
```

If you want to disable Env autocomplete set this to true.

### Enable/Disable Middleware Auto-Completion

```json
"Laraphense.disableMiddlewareCompletion": false
```

If you want to disable Middleware autocomplete set this to true.

### Enable/Disable Mix Auto-Completion

```json
"Laraphense.disableMixCompletion": false
```

If you want to disable Mix autocomplete set this to true.

### Enable/Disable Route Auto-Completion

```json
"Laraphense.disableRouteCompletion": false
```

If you want to disable Route autocomplete set this to true.

### Enable/Disable Translation Auto-Completion

```json
"Laraphense.disableTranslationCompletion": false
```

If you want to disable Translation autocomplete set this to true.

### Enable/Disable Validation Auto-Completion

```json
"Laraphense.disableValidationCompletion": false
```

If you want to disable Validation autocomplete set this to true.

### Enable/Disable View Auto-Completion

```json
"Laraphense.disableViewCompletion": false
```

If you want to disable View autocomplete set this to true.

# Advance Configurations

### Configure Regex for Matching view files

```json
"Laraphense.viewRegex": "(?<=view\\(['\"]|.view:.?['\"]|View::make\\(['\"]|nest\\(['\"](.*)['\"],.?['\"]|@include\\(['\"]|@extends\\(['\"]|@component\\(['\"]|@livewire\\(['\"]|Inertia::render\\(['\"]|\\(component:.['\"]|\\<)(\\<x-|\\<livewire:|[^'\" \\>]+)"
```

this regex is used to match the view files for quick jumping.

### Configure Regex for Creating view files

```json
"Laraphense.viewCreateRegex": "(?<=View::make\\(['\"]|view\\(['\"]|.view:.['\"]|Inertia::render\\(['\"]|\\(component:.['\"])([^'\"]+)"
```

this regex is used to match the view files for auto-suggestion.

### Configure the PHP command like this

```json
"Laraphense.phpCommand": "php -r \"{code}\""
```

this command is used to run PHP for indexing Laravel files.

### Configure the Base path like this

```json
"Laraphense.basePath": "/core"
```

this Base path is used to read files.

### Configure the Code Base path like this

```json
"Laraphense.basePathForCode": "/core/laravel"
```

This base path is used for require_once inside the PHP code.

<!-- ## Known Issues -->

## Credits

-   [PHP parser](https://github.com/glayzzle/php-parser)
-   [mkdirp](https://github.com/isaacs/node-mkdirp)

## Recommended extensions

-   [PHP Intelephense](https://marketplace.visualstudio.com/items?itemName=bmewburn.vscode-intelephense-client)

**Enjoy!**

