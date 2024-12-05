# C# Chromium Browser

An enterprise-grade Chromium-based browser implementation using Microsoft's WebView2 control. This project demonstrates how to create a secure, manageable browser suitable for enterprise environments.

## Features

- Full Chromium engine through WebView2
- Modern web standards support
- Enterprise security features:
  - Automatic HTTPS upgrade
  - Download policy enforcement
  - Security status indicators
  - Certificate validation
- High DPI support
- Comprehensive logging
- Configurable start page

## Prerequisites

- Windows 10 or later
- Visual Studio 2022 (any edition)
- .NET 6.0 SDK
- [WebView2 Runtime](https://developer.microsoft.com/en-us/microsoft-edge/webview2/)

## Quick Start

1. Clone the repository:
   ```bash
   git clone https://github.com/npk-mp/csharp-chromium-browser.git
   cd csharp-chromium-browser
   ```

2. Open `EnterpriseBrowser.sln` in Visual Studio 2022

3. Restore NuGet packages:
   - Right-click solution in Solution Explorer
   - Select "Restore NuGet Packages"

4. Build and run:
   - Press F5 or click "Start" button
   - The browser should launch and load the configured start page

## Configuration

Edit `App.config` to customize:
```xml
<configuration>
  <appSettings>
    <add key="StartPage" value="https://www.google.com"/>
  </appSettings>
</configuration>
```

## Project Structure

```
├── EnterpriseBrowser.sln          # Solution file
├── EnterpriseBrowser/            
│   ├── EnterpriseBrowser.csproj   # Project file
│   ├── Program.cs                 # Entry point
│   ├── MainBrowserWindow.cs       # Main browser implementation
│   ├── App.config                 # Configuration
│   └── Resources/                 # Icons and resources
```

## Development

### Building
```bash
dotnet restore
dotnet build
```

### Running
```bash
dotnet run --project EnterpriseBrowser
```

## Security Features

- Automatic HTTPS upgrade for HTTP URLs
- Security status indicator
- Download policy enforcement
- Certificate validation
- Resource filtering
- Comprehensive logging

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to your branch
5. Create a Pull Request

## License

MIT License - feel free to use this code in your own projects.

## Credits

- Built with [Microsoft.Web.WebView2](https://www.nuget.org/packages/Microsoft.Web.WebView2)
- Based on Chromium engine
