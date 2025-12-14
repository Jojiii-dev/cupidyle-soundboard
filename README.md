# Simple soundboard web app template

Using [Nuxt 3](https://nuxt.com/docs/getting-started/introduction) And [Vuetify](https://vuetifyjs.com/en/introduction/why-vuetify/#feature-guides) as UI library.

## Setup

Make sure to install the dependencies:

package manager: [bun](https://bun.sh/)

```bash
# bun
bun install
```

## Development Server

Start the development server on `http://localhost:3333`:

```bash
# bun
bun run dev
```

## Production

Build the application for production:

```bash
# bun
bun run build
```

Locally preview production build:

```bash
# bun
bun run preview
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.

## How to add Sounds

- add the sound file into one of the folders under cupidyle-soundboard\public\voices
- add an entry to cupidyle-soundboard\assets\voices.json in the group you want it to be under. You can look at the other entries as reference. These entries maps to the buttons on the soundboard
  - path = the path of the sound you added to the cupidyle-soundboard\public\voices directory
  - description = the text shown on the voice button
  - updated_at = UNIX timestamp of then the entry was added, entry within 2 weeks will be shown as "new". You can use this website for current timestamp https://www.unixtimestamp.com otherwise I use a VSCode extension called Timestamper
- Open a pull request for your changes to the main branch, I will review and approve/merge it when I have time
- Once this is done, if you push your changes to the 'main' branch it will automatically trigger an update via Vercel. It should update it to the site in less than a minute
- If you want to test your changes locally you need to install bun using the link at the setup section and follow the setup instructions
