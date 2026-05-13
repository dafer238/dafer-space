# dafer-space

Central repository for space-related projects:

- dafer-astro
- dafer-avionics
- dafer-propulsion

These are included as Git submodules.

---
## Clone (with submodules)

```bash
git clone --recurse-submodules https://github.com/dafer238/dafer-space.git
```

If you already cloned without submodules:
```bash
git submodule update --init --recursive
```

---
## Update all submodules to latest contents in main branch
```bash
git submodule update --remote --merge
```

Then commit the updated pointers:

```bash
git add .
git commit -m "chore(repo): update submodules"
git push
```
---
## Add / initialize submodules manually (dev setup)
```bash
git submodule add -b main https://github.com/dafer238/dafer-astro.git astrodynamics
git submodule add -b main https://github.com/dafer238/dafer-avionics.git avionics
git submodule add -b main https://github.com/dafer238/dafer-propulsion.git propulsion
```
