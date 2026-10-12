# Main Character — Meshy Modeling Brief

## Visual target
Create an original, game-ready masked claw-fighter inspired by the supplied yellow-and-blue reference: yellow/blue tactical trousers, black-and-yellow cowl with swept metal-like side fins, rugged boots, athletic muscular build, and three retractable metal claws on each hand. Treat the supplied picture as visual direction, not as a ready-made 3D model.

Do not label the model as an official Marvel/Wolverine asset or copy protected logos. Make a sufficiently original design for the project.

## Meshy generation prompt
"Create a high-quality, original stylized-realistic 3D video-game hero character, full body, neutral A-pose, symmetrical stance, athletic muscular proportions, wearing a weathered yellow and deep navy-blue tactical combat outfit, reinforced knee panels, black heavy combat boots, a distinctive black-and-yellow full cowl with original swept-back silver side fins that do not obscure the eyes, rugged realistic fabric seams and armor details, six polished retractable metal claws total, three emerging from each fist. PBR materials, clean topology, coherent anatomy, separated material zones, no text, no watermark, no logos, no base, no props, no extra fingers, no extra arms, no duplicated claws. Designed for third-person action game use, readable silhouette, optimized polygon budget, neutral studio lighting."

## Export requirements
- Prefer FBX or GLB supported by the current Unity/ Meshy workflow.
- Include textures and confirm commercial-use rights for the chosen Meshy plan and any generated assets.
- Request or create a humanoid rig and idle, walk/run, jump, attack, and hit animations if available.
- Ensure claws are separate meshes/bones or can be attached to hand sockets.
- Use a consistent scale and apply transforms before import.
- Verify that the model is original enough for the intended use and does not include unauthorized logos.

## Unity integration checklist
1. Import the model and textures under Assets/Characters/MainHero/.
2. Set the model's Rig to Humanoid if its skeleton is compatible; configure avatar mapping.
3. Add an Animator Controller with idle, locomotion, jump, attack and hit states.
4. Replace the procedural player visual in the gameplay bootstrapper with the imported prefab.
5. Keep the existing player movement/collision controller separate from the visual mesh.
6. Attach claw meshes to left/right hand sockets and add a short-range melee hitbox/animation event.
7. Test mobile frame rate, memory, material count, clipping and camera framing.
