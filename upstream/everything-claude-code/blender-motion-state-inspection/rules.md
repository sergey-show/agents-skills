# Rules (extracted)

- Required fix:
- Do not modify body proportions to force pose matching unless the task is explicitly mesh repair.
- Do not bake away the clean baseline before recording it.
- Do not use one rendered camera angle as proof that a pose is correct.
- Do not delete helper objects until you have recorded why they are not part of the character.
- Do not assume an avatar faces +Y, -Y, +X, or -X without checking head, feet, torso, and root motion together.
