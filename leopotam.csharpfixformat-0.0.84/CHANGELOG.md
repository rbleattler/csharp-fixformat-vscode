* v0.0.84
  * Fix backslashes in @-strings.
* v0.0.83
  * Fix enums detection.
* v0.0.82
  * Fix enums with trailing semicolon.
  * Info about default settings at README.
* v0.0.81
  * Upgrade to vscode v1.33 - support for builtin formatter selector.
* v0.0.80
  * Fix destructors formatting.
* v0.0.79
  * Fix double quotes in verbatim strings.
* v0.0.78
  * Fix "in" prefix for C#7.2 readonly reference parameters.
* v0.0.77
  * Fix "ref" prefix for C#7.x variable statements.
* v0.0.76
  * Fix space after fat arrow.
* v0.0.75
  * Fix operator overloading detection.
* v0.0.74
  * Fix nested generics issue.
  * Fix parenthesis issue between logical / bits-shift operators like `t << (16 >> 2)`.
* v0.0.73
  * Fix "goto" behaviour. **SHAME ON ME** for this, this operator should be banned 10 years ago...
* v0.0.72
  * Fix issue on "csharpfixformat.style.spaces.afterParenthesis"=false and next "&&" / "||" / "==".
  * Fix issue on verbatim strings with invalid multiline splitting.
* v0.0.71
  * Fix inconsistent spacing around ":" for multilined named parameters. String consts as field values are not supported!
* v0.0.70
  * README updated: info about omnisharp-vscode extension added.
  * Marketplace tags updated.
* v0.0.69
  * "style.newline.elseCatch" option was added.
* v0.0.68
  * "style.indent.switchCaseIgnored" option was added.
* v0.0.67
  * C#7 "numbers with underscores" support (10_000_000).
* v0.0.66
  * "style.newline.atEnd" option was added.
* 0.0.65
  * Export api object { process, getOptions } through extension.exports.
* 0.0.64
  * Fix #error preprocessor directive.
* 0.0.63
  * Fix "sort.usings.order" issue on multiple lines with different lengths.
* 0.0.62
  * "csharpfixformat.style.operators.onSameLine" option was added.
* v0.0.61
  * Fix #undef preprocessor directive.
* v0.0.60
  * "sort.usings.systemFirst" deprecated, use "sort.usings.order" instead.
* v0.0.59
  * Fix inconsistent spacing around parenthesis with "style.spaces.beforeParenthesis"=false and "csharpfixformat.style.spaces.afterParenthesis"=false.
  * Fix inconsistent spacing around ":" for named parameters.
* v0.0.58
  * "style.spaces.removeAfterCommandBeforeParenthesis" option was added.
* v0.0.57
  * Fix {{ inside interpolation strings.
* v0.0.56
  * Fix #warning preprocessor directive.
* v0.0.55
  * Fix nullable members access.
* v0.0.54
  * Additional fix for nested fields initialization.
* v0.0.53
  * Fix for do_while with "styleBracesOnSameLine"=false.
* v0.0.52
  * Fix for multiple attributes.
* v0.0.51
  * Fix attributes indentation.
* v0.0.50
  * Fix for named parameters detection.
* v0.0.49
  * Additional fix for numeric constants with size suffix.
* v0.0.48
  * Fix for hex strings with number size suffix (e.g. 0x9908b0dfUL).
  * Fix for "UTF-8 with BOM" encoded files in batch mode (force save to "UTF8 without BOM").
* v0.0.47
  * Fix for interpolation strings detection.
* v0.0.46
  * Fix for "<<=" and ">>=" operators.
  * Fix indentation for preprocessor directives / regions when tabs uses.
* v0.0.45
  * Fix issue for mixed line-endings (\r\n + \n) at one file.
  * Description of issues in README updated.
  * Code cleanup.
* v0.0.44
  * Fix operator overloading.
  * Fix named parameters.
* v0.0.43
  * External npm module for recursive file search replaced with builtin function.
* v0.0.42
  * Formatting in batch mode through folder context menu at explorer window.
* v0.0.41
  * Fix issue on spaces.afterParenthesis=true and next opening "(" / "[".
* v0.0.40
  * Fix indentation for enums / nested fields when tabs uses instead of spaces.
* v0.0.39
  * Extension now works as default FormatProvider in vscode (no need custom keybindings / commands).
* v0.0.38
  * Additional fix to number suffixes indentation.
* v0.0.37
  * Fix number suffixes indentation.
* v0.0.36
  * Fix "typeof (" pair with "csharpfixformat.style.spaces.beforeParenthesis"=false.
* v0.0.35
  * Tabs indentation support ("editor.insertSpaces" setting).
* v0.0.34
  * Fix multiple nulable declarations on same line.
  * Revert "Fix body indentation for constrainted generics" due it broken at some cases.
* v0.0.33
  * Fix "$@" combination for strings.
  * Disable formatting for templates inside strings.
  * Fix formatting at readonly editor windows.
  * Fix body indentation for constrainted generics.
  * "csharpfixformat.style.activateDefaultFormatterAfter" option deprecated (prepare to be default formatter).
* v0.0.32
  * Fix foreach loop without parentheses.
* v0.0.31
  * Fix commented string templates.
* v0.0.30
  * Performance fix for nested fields initialization.
* v0.0.29
  * Compatibility with vscode 1.14 and new marketplace rules.
* v0.0.28
  * Additional fix for nested fields initialization.
* v0.0.27
  * Fix nested fields initialization.
* v0.0.26
  * Fix for #elif formatting.
* v0.0.25
  * Fix double quotes inside interpolated strings.
* v0.0.24
  * Fix #pragma definitions.
* v0.0.23
  * Fix C#7 "out var variable" syntax.
* v0.0.22
  * Fix escaped template strings.
* v0.0.21
  * Fix multiline strings.
* v0.0.20
  * Fix nested generics.
* v0.0.19
  * Fix "> (" and "> [" pairs with options spaces.beforeParenthesis=false / spaces.beforeBracket=false.
* v0.0.18
  * Fix const declaration with access modifier.
  * Improve string / char sequences recognition.
* v0.0.17
  * Fix invalid generics processing on complex condition expressions.
  * Fix formatting of "> )", "> ]", "> (", "> [" and "> ;" pairs.
  * "csharpfixformat.csharpfixformat.style.spaces.beforeIndexerBracket" option was added.
    > Override spaces.beforeBracket rule for indexer sequence 'this['.
* v0.0.16
  * Fix generics processing.
  * Readme.md badges.
* v0.0.15
  * Fix force new line for yield.
  * Fix force new line for default(T).
  * Fix processing double quotes inside string.
* v0.0.14
  * Fix for escaped strings formatting (double quotes and @ prefix).
  * /\* fixformat ignore:start \*/ and /\* fixformat ignore:end \*/ directives added
  for ignore formatting between them.
  * Refactoring.
* v0.0.13
  * Fix for string interpolators formatting.
  * Code cleanup.
* v0.0.12
  * "csharpfixformat.style.spaces.beforeBracket" default value changed to false.
  * Fix for #region / endregion formatting.
  * "csharpfixformat.style.indent.regionIgnored" option was added.
    > Should #region / #endregion directives ignore indentation or use it.
* v0.0.11
  * All style reformatting respect single line / multiline comments and strings.
  * Fix for preprocessor directives started from "!".
  * Fix for "braces.allowInlines"=true for multiple expressions in line.
  * Fix closing brace indentation for enums.
  * Improve internal error processing.
* v0.0.10
  * Keybinding "ctrl+alt+i" was added for formatting activation.
  * "csharpfixformat.style.activateDefaultFormatterAfter" option was added.
    > Should default code formatter be activated as post process.
  * "csharpfixformat.style.braces.onSameLine" option was added.
    > Should open braces be kept on expression line (K&R style) or on new line.
  * "csharpfixformat.style.braces.allowInlines" option was added.
    > Allow expressions inside braces at one line.
  * "csharpfixformat.style.spaces.beforeParenthesis" option was added.
    > Space before '(' - opening parenthesis.
  * "csharpfixformat.style.spaces.afterParenthesis" option was added.
    > Space after ')' - closing parenthesis.
  * "csharpfixformat.style.spaces.beforeBracket" option was added.
    > Space before '[' - opening bracket.
  * "csharpfixformat.style.spaces.afterBracket" option was added.
    > Space after ']' - closing bracket.
  * "csharpfixformat.style.spaces.insideEmptyParenthis" option was added.
    > Space inside '()' - empty parenthis.
  * "csharpfixformat.style.spaces.insideEmptyBraces" option was added.
    > Space inside '{}' - empty braces.
  * "csharpfixformat.style.spaces.insideEmptyBrackets" option was added.
    > Space inside '[]' - empty brackets.
  * Fix colons / generics formatting.
  * Fix usings sorting as one block after splitting.
* v0.0.9
  * Code style code was removed, js-beautify uses instead.
  * Sort using can be disabled.
  * Code style formatting can be disabled.
  * Config options were refactored.
  * "csharpfixformat.sort.usings.enabled" option was added.
    > Should usings be sorted or not.
  * "csharpfixformat.sort.usings.systemFirst" option was added.
    > Put System.xxx namespaces first at usings list on sorting.
  * "csharpfixformat.sort.usings.splitGroups" option was added.
    > Insert blank line between using blocks grouped by first part of namespace.
  * "csharpfixformat.style.enabled" option was added.
    > Enable code reformat with style options.
  * "csharpfixformat.style.newline.maxAmount" option was added.
    > Amount of new line (\n) symbols allowed in row. 1 means no blank lines. Use 0 for disable.
  * "csharpfixformat.style.indent.preprocessorIgnored" option was added.
    > Should preprocessor directives ignore indentation or use it.
* v0.0.8
  * Sort usings logic fixes, doubles in usings will be removed automatically.
  * Warning notification was added.
  * Indentation fixes for multiline assign expressions.
  * Performance fix for indentEnabled = false.
  * tslint fixes.
* v0.0.7
  * Indentation fix for content after single line comments with "{", "(", etc.
* v0.0.6
  * Correct sorting of using lines with chars in different cases (like "S" and "s").
  * "csharpfixformat.indentPreprocessor" option was added.
    > Indent preprocessor defines or put them without indentation. Disable by default.
* v0.0.5
  * Switch-case indentation fixed.
* v0.0.4
  * Comment skipping. Dont use tail comments at using line - they will be removed!
  No limits for other places for tail comments.
  * Indent of wrapped lines with not finished assign expression should be fixed.
* v0.0.3
  * "Sort usings" command renamed to "Fix format".
  * "csharpfixformat.indentEnabled" option was added.
    > Indent all lines with respect of parentheses / braces and use "editor.tabSize" parameter. Enabled by default.
  * "csharpfixformat.emptyLinesInRowLimit" option was added.
    > Amount of empty lines in row, negative value for disable. By default 1 empty line allowed between expressions.
  * Sort usings should works correctly for multiple using expressions in line.
  * Sort usings should ignore commented expressions (if usings put at begining of each line inside multiline comment - they will be sorted).
  * Refactoring.
* v0.0.2
  * Debug logging removed.
  * Refactoring.
* v0.0.1
  * Init release.