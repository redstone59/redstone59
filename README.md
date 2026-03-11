```py
from dataclasses import dataclass

@dataclass
class PersonThings:
    name: str = "redstone59"
    pronouns: tuple[str, str] = ("she", "her")
    language_proficency: dict[str, str] = {
        "Python": "fluent",
        "C#": "fluent",
        "TypeScript": "surprisingly alright at it",
        "JavaScript": "decent",
        "C": "haven't touched in ages"
    }
    currently_enjoys: list[str] = [
        "Starting a bunch of new projects that don't really get anywhere.",
        "Learning TypeScript",
        "Messing with my Obsidian Vault"
    ]
    currently_dislikes: list[str] = [
        "Starting a bunch of new projects that don't really get anywhere.",
        "Looking at old projects (I've gotten a lot better at programming over the past five years)"
    ]
```

```cs
namespace CurrentProjects
{
    public struct Project
    {
        public string description;
        public string[] languages;
        public string? link; // I typically have repositories private until they are functional. Sorry!
    }

    public Project nineCircle = new(
        "An -le game (like Wordle) based on the many Nine Circles clones in Geometry Dash",
        ["TypeScript", "HTML/CSS"],
        "https://github.com/redstone59/Nine-Circ-le"
    );
}
```

```ts
class Project {
    name: string;
    description: string;
    probable_languages: string[]
}

const projectsImConsidering: Project[] = [
    {
        name: "LadderRank",
        description: "A website where users can rank media on a ladder from best to worst using binary search with less emphasis on a number rating.",
        probable_languages: ["TypeScript", "HTML/CSS"]
    },
    {
        name: "Scribousel",
        description: "A collaborative story-writing web browser game. Idea inspired by the video 'Markiplier Makes: Fan Fiction' by Markiplier.",
        probable_languages: ["Python", "TypeScript", "HTML/CSS"]
    }
]
```
