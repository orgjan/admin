# VS Code Configuration for C/C++ Development

This directory contains configuration files to enable C/C++ syntax analysis and IntelliSense in Visual Studio Code.

## Files

### settings.json
Workspace settings for C/C++ extension:
- Enables error squiggles (red underlines for syntax errors)
- Configures IntelliSense engine to default mode
- Sets C++17 and C11 standards as defaults
- Enables autocomplete and code snippets

### c_cpp_properties.json
C/C++ IntelliSense configuration:
- Configures include paths for different platforms (Linux, Windows, Mac)
- Sets compiler paths for each platform
- Defines C/C++ standards (C11 and C++17)
- Configures IntelliSense modes for different compilers

### extensions.json
Recommended extensions:
- `ms-vscode.cpptools` - Official C/C++ extension from Microsoft
- `ms-vscode.cpptools-extension-pack` - C/C++ Extension Pack with additional tools

## Usage

1. Install the recommended C/C++ extension from Microsoft:
   - Open VS Code
   - Press `Ctrl+Shift+X` (or `Cmd+Shift+X` on Mac)
   - Search for "C/C++"
   - Install "C/C++" by Microsoft

2. Reload VS Code to apply the configuration

3. Open any C/C++ file - syntax highlighting and error checking should now work automatically

## Troubleshooting

If syntax analysis is not working:
1. Make sure the C/C++ extension is installed and enabled
2. Check the Output panel (View → Output) and select "C/C++" from the dropdown
3. Verify that the compiler path in `c_cpp_properties.json` matches your system
4. Try reloading the VS Code window (Ctrl+Shift+P → "Developer: Reload Window")

## Customization

You can customize these settings by:
- Editing `settings.json` for workspace-specific C/C++ settings
- Modifying `c_cpp_properties.json` to adjust include paths or compiler settings
- Adding your own compiler paths and configurations
