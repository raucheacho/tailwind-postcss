# tailwind-postcss

1. Clonez le repositorie et lancez la commande.
    >npm install

2. pour compiler la version dev de tailwind lancez:
    >npm run build

3. pour compiler la version dev de tailwind lancez:

    >npm run purge

    ```
    configurez la partie purge de postcss dans 
    postcss.config.js

    purgecss({
      content: ["./src/templates/**/*.html"], # configurez le dossier de fichiers html.
      defaultExtractor: content => content.match(/[\w-/:]+(?<!:)/g) || []
    })

    ```