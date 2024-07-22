```py
from dataclasses import dataclass

@dataclass
class PersonThings:
    name: str = "redstone59"
    pronouns: tuple[str, str] = ("she", "her")
    language_proficency: dict[str, str] = {
        "Python": "fluent",
        "C#": "semi-fluent",
        "TypeScript": "surprisingly alright at it",
        "JavaScript": "decent",
        "C": "haven't touched in ages"
    }
    currently_enjoys: list[str] = [
        "Rewriting old projects",
        "Learning TypeScript",
        "the Unity game engine"
    ]
    currently_dislikes: list[str] = [
        "Looking at old projects (I've gotten a lot better at programming over the past year)",
        "the Unity game engine"
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
        ["TypeScript", "TSX (React)"], // A good friend of mine is doing all the front-end.
        "https://github.com/redstone59/Nine-Circ-le"
    );

    public Project backshotRouletteRewrite = new(
        "A bot that finds the best move in a game of Buckshot Roulette. Again. But written LIVE!!! ON STREAM!!!",
        ["Python"],
        "https://github.com/redstone59/BackshotRoulette"
    );

    public Project buckshotGameNotation = new(
        "An adapation of Chess' *algebraic notation* to Buckshot Roulette.",
        ["GDScript", "Python"],
        null
    )
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
        name: "Some kind of Buckshot Roulette all-in-one program",
        description: "A BGN editor with evaluation capabilities with a bot of choice (in this case, Backshot Roulette). I've already devised the Buckshot Bot Interface so the program can communicate with other bots, too. Maybe it'd be a mod onto Buckshot Roulette (I do use Godot on occasion, a mod surely couldn't be that hard)",
        probable_languages: ["Python", "GDScript"]
    },
    {
        name: "mCmd", // working title
        description: "A higher-level language that transpiles to [LazyCMD](https://github.com/redstone59/LazyCMD). Considering making it Pythonic instead of C-like (too many C-like command block languages exist)",
        probable_languages: ["Python"]
    }
]
```
