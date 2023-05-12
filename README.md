# PythonScriptModifierTemplate
Template for a custom Python script modifier that hooks into OVITO.

This repository contains a template to create your own Python script modifier which can be install into OVITO using pip. 

## Getting Started

1. Click the "Use this template" button to create a new repository.
1. Rename src/ModifierName to reflect the name of your modifier.
2. Rename `ModifierName` to the name of your module and modifier class and implement its modify method.
3. If your modifier needs access to more than one frame or frames from an external trajectory you can uncomment and implement the `input_caching_hints` method. More details on this method can be found in the [OVITO documentation](https://www.ovito.org/docs/current/python/introduction/custom_modifiers.html#writing-custom-modifiers-advanced-interface). Otherwise, you can delete it.
4. Fill in the pyproject.toml file. Fields that need to be updated are enclosed in a descriptive `[[field]]` tag. If your Python package has additional dependencies, you can uncomment the example dependency section. Depending on your needs, you can add additional fields to the pyproject.toml file. Information can be found [here](https://setuptools.pypa.io/en/latest/userguide/index.html).
5. Fill in the README_Template.md file the [[fields]] should guide you. Feel free to add other sections like "Images", "Citation", or "References" as needed.
6. Add meaningful examples to the Examples directory to help others understand the use of your modifier.
7. Pick a license for you project and replace the current (MIT) LICENSE file with your license. If you keep the MIT license please update the name and year in the current file.
8. Once you're done rename README_Template.md to README.md, replacing this file.
