# Run Blazor with the command line (CLI)

You can run this Blazor app entirely from the terminal. **You do not need the VS Code C# extension** or any IDE—the .NET CLI is enough.

## Prerequisites

- **.NET SDK** (includes `dotnet` CLI).  
  - Check: run `dotnet --version` in a terminal.  
  - Install: [Download .NET](https://dotnet.microsoft.com/download) (choose SDK for your OS).

## Steps

1. **Open a terminal** in the project root.

2. **Restore packages** (first time or after pulling changes):
   ```bash
   dotnet restore
   ```

3. **Build the project**:
   ```bash
   dotnet build
   ```

4. **run with hot reload**

To rebuild and reload when you change code without restarting manually:

```bash
dotnet watch run
```

Leave this running while you edit; the app will refresh after changes.

5. **Open in a browser**  
   When it starts, the app will show URLs in the terminal. Use:
   - **HTTP:** [http://localhost:5049](http://localhost:5049)
   - **HTTPS:** [https://localhost:7058](https://localhost:7058)  
   (HTTPS may show a certificate warning in the browser; you can proceed for local development.)

6. **Stop the app**  
   Press `Ctrl+C` in the terminal.
   