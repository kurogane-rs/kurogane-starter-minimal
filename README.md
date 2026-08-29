# Kurogane: Vanilla starter

A minimal Kurogane application with no frontend framework. Just HTML, CSS and TypeScript or JavaScript.

## Supported Languages

- `typescript`: TypeScript with Vite's built-in esbuild transform
- `javascript`: Good 'ol JavaScript

## Usage with Kurogane CLI

```sh
kurogane new minimal
```

Select a language when prompted.

## Non-interactive usage

```sh
cargo generate kurogane-rs/starter-minimal --name my-app --define language=typescript
```

## What's included

- Minimal `index.html` with entry point
- Vite configured to build into `content/`
- Rust binary using the Kurogane runtime
- `kurogane.toml` packaging configuration

## Development

```sh
npm install
npm run dev    # Start Vite dev server (port 5173)
kurogane dev   # Launch the Kurogane desktop app
```

## Building

```sh
npm run build      # Build frontend
kurogane build     # Build the Rust binary
```

## TypeScript vs JavaScript

The TypeScript variant includes `main.ts` and TypeScript dev dependencies. The JavaScript variant includes `main.js` with no TypeScript tooling. Both produce identical functionality.
