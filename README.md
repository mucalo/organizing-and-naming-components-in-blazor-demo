# Organizing and Naming Components in Blazor

Demo project to go with the Organizing and Naming Components in Blazor article on my blog:
https://mariomucalo.com/organizing-and-naming-components-in-blazor

My basic rules are:

- have the view and the code behind in two separate files
- the code behind file is named the same as the view file with the _.razor.cs_ extension - this will allow nesting of files in the Visual Studio IDE
- I use Razor components for both Pages and Components. I put pages in the _/Pages_ folder and components in the _/Components_ folder (or in a separate Razor Class Library).
- Pages are components that can be accessed via URL - meaning they have the ``` @page "/my-route-here" ``` annotation. The file name should contain Page in the end (e.g. _IndexPage.razor_)
- Components need to have Component in the file name (e.g. _MyDemoComponent.razor_)
