# p32929 on OpenStore

> **Want to list your own apps?** Start from this repo's [`template` branch](https://github.com/p32929/p32929_openstore/tree/template); this `main` branch is my real listing, an example.

My OpenStore listing. Every `.md` file in [`apps/`](apps/) is an app (its file name becomes its link); [`profile.yaml`](profile.yaml) is optional.

Before pushing, check everything:

```bash
node validate.mjs
```

Push a change and the store picks it up on its next build.
