# Wrapper

Wrapper is way to display views or content by vertically wrapping them in a horizontal pattern.

# Requirements
* iOS 14 or 
* macOS 11

# Installation
There are two ways to add to your own project
1. Add as a Swift Package Dependency 
2. Import this project into your Xcode project and add under Frameworks and Libraries. 

```http
https://github.com/jonnyholland/Wrapper
````

# Use
Simply import Grid, then use as seen below. 

````swift
import Grid
````
````swift
static let imageNames: [String] = ["plus",
"minus",
"person",
"trash",
"doc",
"paperplane",
"newspaper"]
````
````swift
Grid(imageNames) { imageName in
Image(systemName: imageName)
}
````

## Customize
You can actually customize every aspect of the grid so the items are arranged and displayed according to your liking.
````swift
Grid(imageNames, minimumWidth: 100, padding: 10, spacing: 15) { imageName in
Image(systemName: imageName)
}
````
