# Last Circle — Battle Royale

Unity 6 starter project for a third-person battle-royale prototype, with a Vercel static-hosting scaffold.

## Important status

- This repository's root is configured for a Vercel static deployment.
- **This is not yet a playable browser build.** Vercel does not compile Unity projects.
- Export a Unity WebGL build before expecting the game to run in a browser.
- The current Unity starter uses procedural placeholder geometry; it does not yet include a finished Wolverine-inspired rigged model, production-quality assets, or online multiplayer.
- The character reference should be used to create an original, properly licensed model in Meshy; the reference image itself is not a 3D asset.

## Unity project

The Unity project ZIP supplied with this project is named `LastCircle-Unity-Project.zip`. Extract it and open the project folder in Unity 6. In Unity, use **Last Circle → Build Battle Royale Scene**, then save and test the scene. This Git repository currently contains the web deployment scaffold; upload the Unity source files separately if they are not yet present here.

## Vercel setup

1. Import this public GitHub repository into Vercel.
2. Framework preset: **Other**.
3. Build command: leave blank.
4. Output directory: `.` (repository root).
5. Deploy.

This first deployment serves the project status page only. It does not mean the game is playable yet.

## Add the Unity WebGL build

1. In Unity, install WebGL Build Support for your Unity editor version.
2. Switch the project to **Web** / **WebGL** in Build Profiles and build.
3. Put the exported browser build under `public/game/` (or adjust Vercel's output directory and paths accordingly). Include the generated loader JavaScript, framework JavaScript, `.wasm`, and `.data` files.
4. Add a Unity WebGL loader to `index.html` that loads the generated build. Configure the template to match the actual generated filenames; do not guess filenames.
5. Commit and push. Vercel will redeploy from GitHub automatically.

Large WebGL data files may exceed GitHub's ordinary file-size limits. If that happens, use Git LFS or a suitable artifact/CDN hosting approach and verify Vercel's limits before deployment.

## Planned milestones

- [ ] Upload complete Unity source and project settings
- [ ] Create an original rigged, animated main-character model and import it
- [ ] Replace proxy geometry with licensed environment/weapon/character assets
- [ ] Test gameplay and mobile controls in Unity
- [ ] Build and test WebGL on desktop and mobile browsers
- [ ] Add multiplayer only after the single-player loop is stable

## License and assets

Do not redistribute third-party assets unless their license explicitly allows it. Add license notices for all imported models, animations, sounds, and textures.