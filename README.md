# One Click Away

Unity game project.

## Requirements

- Unity `6000.5.3f1` (Unity 6)
- A desktop platform supported by Unity
- Git, if you are cloning the repository from GitHub

The project uses the Universal Render Pipeline and restores its Unity packages
from `Packages/manifest.json` and `Packages/packages-lock.json`.

## Get Started

1. Clone or download this repository.
2. Open Unity Hub and select **Add > Add project from disk**.
3. Select the repository folder, the folder containing this README.
4. Open it with Unity `6000.5.3f1`.
5. Wait for Unity to import assets and resolve packages.
6. Open `Assets/Scenes/SampleScene.unity` and press **Play**.

Unity may take a few minutes to recreate the local `Library` cache on the first
open. That folder is intentionally excluded from Git.

## Scenes

- `Assets/Scenes/SampleScene.unity`: default scene included in the build.
- `Assets/Scenes/One Click Away.unity`: project scene available for testing.
- `Assets/Scenes/ZNS3D/Vintage Living Room Game Pack/Demo/Demo_Scene.unity`:
  asset-pack demonstration scene.
- `Assets/Scenes/ZNS3D/Vintage Living Room Game Pack/Demo/All_Prefabs.unity`:
  asset preview scene.

To change the scene used by a build, open **File > Build Profiles** and update
the scene list. The current build configuration includes `SampleScene`.

## Input

The Unity Input System action asset is
`Assets/InputSystem_Actions.inputactions`. Its `Player` action map contains
`Move`, `Look`, `Attack`, `Interact`, `Crouch`, `Jump`, `Previous`, `Next`, and
`Sprint` actions. Review the bindings in the Input Actions editor before
changing controls or adding a new player object.

## Repository Layout

- `Assets/`: scenes, models, textures, prefabs, and Unity assets.
- `Packages/`: package manifest and lock file.
- `ProjectSettings/`: Unity editor and project configuration.
- `.vscode/`: workspace settings for VS Code.

Generated folders such as `Library`, `Temp`, `Logs`, `Obj`, `Build`, and
`UserSettings` are excluded because Unity recreates them locally. Generated IDE
solution and project files are also excluded.

## Troubleshooting

- If Unity reports package or import errors, confirm the project is opened with
  Unity `6000.5.3f1` and allow the Package Manager to finish resolving.
- If the project opens with missing or stale cached data, close Unity and remove
  the local `Library` folder, then reopen the project.
- If a scene is not included in a build, add its `.unity` file in **Build
  Profiles**.

done by aser sameh