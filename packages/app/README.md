# App Challenge

> Place your project in `packages/app/`.

## Tasks

1. Set up a SvelteKit project with
  - Tailwind
  - Open Sans ([`@font-source/open-sans`](https://www.npmjs.com/package/@fontsource/open-sans) is a pretty cool package)
  - Colours
    - #1CB569
    - #0D8767
    - #095D4F
    - #4A90E2
    - #5E62A3
    - #383A61
    - #3F495A
    - #647490
    - #8494AD
    - #A0ADC0
2. Implement a home page
  - Move re-used elements to a components folder (component library)
3. Implement a profile list page
  - Query https://api-staging.linguala.com/graphql with [houdini](https://www.npmjs.com/package/houdini)
  - Display some amount of profiles on first load
  - Implement a button to load more profiles after the fact
  - Implement a way to filter profiles by service group
    > TODO: add available groups 
4. Implement a profile page & link to it from the list page
  > You can use the id as the slug.
