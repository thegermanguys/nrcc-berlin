# lib/players/ — Player Photo Library

Place player photos in this folder.
The filename **must match** the `photoFile` field in `squad.html`.

## Naming Convention

| Player Name       | Filename              |
|-------------------|-----------------------|
| Awanish           | `awanish.jpg`         |
| Rajan Thapa       | `rajan-thapa.jpg`     |
| Bikash Karki      | `bikash-karki.jpg`    |
| Sanjay Rai        | `sanjay-rai.jpg`      |
| Dipesh Shrestha   | `dipesh-shrestha.jpg` |
| Nabin Tamang      | `nabin-tamang.jpg`    |
| Roshan Gurung     | `roshan-gurung.jpg`   |
| Sunil Magar       | `sunil-magar.jpg`     |
| Pranav Subedi     | `pranav-subedi.jpg`   |
| Aakash Adhikari   | `aakash-adhikari.jpg` |
| Suresh Lama       | `suresh-lama.jpg`     |
| Bijay Bista       | `bijay-bista.jpg`     |

## Rules
- Use lowercase, hyphens for spaces (no underscores, no spaces)
- Supported formats: `.jpg`, `.jpeg`, `.png`, `.webp`
- Recommended size: **400×400px** minimum, square crop works best
- If a photo file is missing, the player card falls back to the emoji icon

## Adding a New Player
1. Add their photo to this folder: `lib/players/firstname-lastname.jpg`
2. Add their entry to the `players` array in `squad.html`:
   ```js
   { name:"First Last", role:"Batsman", emoji:"🏏", captain:false, photoFile:"first-last.jpg" },
   ```
