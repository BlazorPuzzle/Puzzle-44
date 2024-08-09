# Blazor Puzzle #44

## No RCL Protection!

YouTube Video: https://youtu.be/ZBCaNIfrxsw

Blazor Puzzle Home Page: https://blazorpuzzle.com

### The Challenge:

This a .NET 8 Blazor Web App with Global Server Interactivity. We are using Protected Local Storage to store encrypted data in the browser space.

For information on this, [see the repo for episode 35](https://github.com/BlazorPuzzle/puzzle-35).

The challenge is to use Protected Local Storage in a Razor Class Library, so the code can be shared by other areas of the application, but it doesn't work!

How can we use Protected Local Storage in an RCL?

### The Solution:

The solution is simple. Add the following package reference to the *Puzzle-44.Shared.csproj* file:

```html
<PackageReference Include="Microsoft.AspNetCore.Components.WebAssembly.Server" Version="8.0.7" />
```

Sometimes, a package is just a package...

Boom!

