# JavaFX Template

A simple template for building a JavaFX app.

## Usage

Download this code by using the download button or [clicking here](https://github.com/Noskcaj19/javafx-template/archive/master.zip) and unzip it a place of your choosing.

Then, open it in your editor or IDE:

### VSCode

[You can download VSCode here](https://code.visualstudio.com/docs/java/java-tutorial#_installer-of-visual-studio-code-for-java-developers):

- Ensure your have installed the [Java Extension Pack](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack) ([see here for help](https://code.visualstudio.com/docs/editor/extension-gallery))
- Ensure you have a Java JDK installed. (Recommended sources: [Oracle OpenJDK](https://jdk.java.net/) or [AdoptOpenJDK](https://adoptopenjdk.net/))

Open the javafx-template folder you extracted, you should soon see a message "The workspace contains Java projects. Would you like to import them?", select "Yes" or "Always".

Navigate to `src/main/java/com/example/App.java`, and there should be a `Run` button above the `main` function.

If you are asked if you want to switch to "Standard mode", select yes.

### Intellij IDEA

[You can download Intellij IDEA here](https://www.jetbrains.com/idea/download) (make sure to download community or register as a student to get Ultimate for free)

- Ensure you have a Java JDK installed. (if you do not have a JDK installed, Intellij can automatically download one for you [instructions here](https://www.jetbrains.com/help/idea/sdk.html#define-sdk)) (or manual instalation from [Oracle OpenJDK](https://jdk.java.net/) or [AdoptOpenJDK](https://adoptopenjdk.net/))).

On the Intellij IDEA start page, select "Open or Import", and select the javafx-template folder you extracted.
Navigate to `src/main/java/com/example/App.java`, and there should be a `Run` button next to the line numbers next to the `main` function.

### Eclipse

- Select "Import projects..."
- Select "General > "Projects from Folder or Archive"
- Click "Directory" and choose the folder the javafx-template folder you extracted.
- Select finish.

### Other IDEs

This template should also "just work" for IDEs, although it has not been tested.

### Finally

You can rename the package (ensure you change the package name in `module-info.java` as well, although using your editors refactoring ability should be easier)

#### Technical notes

This template uses Java 9 Modules to make it easier to configure JavaFX more easily, with the line ` requires transitive javafx.controls;`.
To convert this to a non-modular project, you _must_ add `--module-path /path/to/JavaFX/lib --add-modules=javafx.controls` to your VM options (how this is done depends on your IDE or editor).
