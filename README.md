# Interactive Skill Map

This project is a dynamic and interactive visualization of a personal skill set, built with D3.js. It's designed to be an engaging and visually appealing alternative to a traditional list on a resume or portfolio.

The map is fully configured via a single JSON file, making it easy for anyone to fork this project and create their own skill map.

![Skill Map Demo](https://i.imgur.com/uR13V8G.gif)
*(You can replace this with a screenshot or GIF of your own skill map!)*

## Features

- **Interactive Graph:** A force-directed graph that you can interact with.
- **Zoom & Pan:** Zoom in on specific skills or pan around the entire map.
- **Click for Details:** Click on any skill node to see details like proficiency, a description, and related projects.
- **Customizable Layout:** Hold `Ctrl` (or `Cmd` on Mac) and drag nodes to permanently save their position.
- **Easy to Edit:** All content is driven by the `skillTreeData.json` file. No coding required to update your skills.

## How to Use

You can create your own skill map in just 3 easy steps:

#### 1. Fork this Repository

Click the "Fork" button at the top-right of the GitHub page to create your own copy of this project.

#### 2. Edit `skillTreeData.json`

This is the only file you need to edit to customize the map with your own skills. Open `skillTreeData.json` and modify the structure.

The JSON format is a nested tree. Here's a basic example:

```json
{
  "name": "Software Engineering",
  "children": [
    {
      "name": "Frontend",
      "color": "#4ade80",
      "children": [
        {
          "name": "React",
          "proficiency": 4,
          "blurb": "Proficient in building complex, stateful applications using modern React features.",
          "projects": [
            {
              "name": "My Awesome Project",
              "url": "[https://github.com/your-username/your-repo](https://github.com/your-username/your-repo)"
            }
          ]
        }
      ]
    }
  ]
}