# UIRenderer (https://github.com/yeekitc/UIRenderer)

A custom UI Renderer implemented from scratch, featuring hierarchical UI models, efficient damage/redraw mechanisms, and flexible layout management using springs & struts paradigms.

## Features

- **Hierarchical Rendering System**: UI components are organized in a hierarchy, allowing recursive rendering and parent-child relationships.
- **Damage/Redraw Mechanisms**: Efficiently track and redraw only affected areas.
- **Layout Management**: Uses springs & struts layout models to arrange UI components.

## How to Use

Since the renderer requires running over HTTP(S), set up a local web server to serve the project files. The Live Server extension on VS Code is an option. Then run `index.html` in the `out/` directory to start.

## Project Structure

- **`src/`**: 
  - **`DrawnObjectBase.ts`**: Base class for drawable objects in the UI.
  - **`FilledObject.ts`, `TextObject.ts`, `IconObject.ts`, `DrawableImage.ts`**: Various subclasses that extend `DrawnObjectBase` to represent specific visual components.
  - **`Spring.ts`, `Strut.ts`, `SizeConfig.ts`**: Classes for layout management, defining flexible and fixed-size layout components.
  - **`Row.ts`, `Column.ts`, `Group.ts`**: Classes to handle grouping and arrangement of UI elements.
  - **`test_cases.ts`**: Contains various test cases to validate the UI renderer's behavior and functionality.
- **`out/index.html`**: Entry point for running the renderer in a browser, linking the transpiled JavaScript and other assets.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
