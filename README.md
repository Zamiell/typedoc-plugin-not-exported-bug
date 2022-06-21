# typedoc-plugin-not-exported-bug

Steps to reproduce:

- `git clone git@github.com:Zamiell/typedoc-plugin-not-exported-bug.git`
- `cd typedoc-plugin-not-exported-bug`
- `npm ci`
- Observe how `src/index.ts` and `src/someFile.ts` look.
- `npx typedoc`
- Observe how the generated docs look. The docs have the following symbols:
  - `thing1`
- However, the docs *should* have the following symbols:
  - `thing1`
  - `thing2`
  - `Foo`
