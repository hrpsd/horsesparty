# Horses Party
Horses Party is an hypercasual **children's game** for **touch devices** featuring ponies and unicorns. It is made with Unity 3D.

You can play the **Web** version here: [Horses Party WebGL](https://fartingponies.github.io/horsesparty)

You can play the **Android** version here: [Horses Party Android](https://play.google.com/store/apps/details?id=com.fartingponies.horsesparty)

You can play the **iOS** version here: [Horses Party iOS](https://apps.apple.com/fr/app/horses-party/id6446471793)

## About the characters animation scheme
This project started with the requirements of reusing vector, frame by frame horses animations from the Adobe Flash era. The game is currently using the Unity vector graphics package to avoid handling a huge atlas for the characters. But Unity can't animate vector sprites as it does with 2D sprites, because every SVG animation frame is imported as a GameObject which possibly includes his own atlas for the gradients.
This led me to the shameful choice of enabling the current character frame GameObject at every Update.

## Known Code Issues
- Use of public fields instead of private serialized fields or properties
- Use of a static game manager instead of scriptable objects

## License

Copyright (C) 2023-2026 Sylvain Nowé

Horses Party is free software, licensed under the GNU Affero General Public
License v3.0 or later (see [LICENSE](LICENSE)), with an additional permission
for the Unity engine. Earlier versions were released under the GPL v3.
Third-party assets are excluded: see [NOTICE.md](NOTICE.md).
