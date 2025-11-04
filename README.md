# Ntech.MVVM.Prism Sample Application

This is a sample WPF application demonstrating the implementation of MVVM architecture using Prism Framework. The project showcases modular application development with loosely coupled components.

## Project Structure

The solution consists of multiple projects:

- **Prism.Sample.Demo**: Main application project (WPF)
  - Contains the application shell and bootstrapper
  - Manages module loading and dependency injection
  - Target Framework: .NET Framework 4.8

- **Prism.Sample.ModuleA**: Sample module implementation
  - Contains `AModule`, `AView`, and `AViewModel`
  - Demonstrates basic module structure

- **Prism.Sample.ModuleB**: Sample module implementation
  - Contains `BModule`, `BView`, and `BViewModel`
  - Showcases module independence

- **Prism.Sample.ModuleC**: Sample module implementation
  - Contains `CModule`, `CView`, and `CViewModel`
  - Example of modular functionality

- **Prism.Sample.ModuleD**: Sample module implementation
  - Contains `DModule`, `DView`, and `DViewModel`
  - Demonstrates module isolation

## Technologies & Frameworks

- **WPF (Windows Presentation Foundation)**
- **Prism 4.0.0.0**: MVVM Framework
- **Unity 2.0**: Dependency Injection Container
- **.NET Framework 4.8**

## Key Dependencies

- Microsoft.Practices.Prism (4.0.0.0)
- Microsoft.Practices.Prism.UnityExtensions (4.0.0.0)
- Microsoft.Practices.Unity (2.0)
- Microsoft.Practices.ServiceLocation (1.0)

## Project Features

1. **Modular Architecture**
   - Loose coupling between modules
   - Independent module development
   - Easy to add/remove modules

2. **MVVM Implementation**
   - Separation of concerns
   - View-ViewModel binding
   - Command pattern implementation

3. **Dependency Injection**
   - Unity container integration
   - Service location
   - Interface-based development

## Getting Started

1. **Prerequisites**
   - Visual Studio 2017 or later
   - .NET Framework 4.8 SDK
   - NuGet Package Manager

2. **Build and Run**
   - Clone the repository
   - Open `Prism.Sample.Demo.sln` in Visual Studio
   - Restore NuGet packages
   - Build the solution
   - Run the application

## Solution Architecture

```
Prism.Sample.Demo/
├── App.xaml                 # Application entry point
├── BootStrapper.cs         # Prism bootstrapper configuration
├── PrismShell.xaml         # Main application shell
└── ModuleX/               # Each module follows similar structure
    ├── XModule.cs         # Module initialization
    ├── View/              # XAML views
    └── ViewModel/         # View models
```

## Development Guidelines

1. **Adding New Modules**
   - Create a new class library project
   - Implement IModule interface
   - Register in bootstrapper
   - Follow MVVM pattern

2. **Module Communication**
   - Use event aggregation
   - Implement loose coupling
   - Avoid direct references between modules

3. **Dependency Injection**
   - Register services in module initialization
   - Use constructor injection
   - Follow interface-based design

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contributors

- ntechdevelopers

## Acknowledgments

- Prism Library Team
- Microsoft WPF Team
