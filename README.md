# Rollup

This work is devoted to God.

## Installing

```sh
npm install --global rollup @rollup/plugin-commonjs rollup-plugin-node-polyfills
```

## Building

### For Browser

```sh
rollup main.js --file bundle.js --format es --plugin commonjs --plugin node-polyfills
```

### For Node.js

```sh
rollup main.js --file bundle.js --format cjs --plugin commonjs
```

## ZSH Function

```zsh
build() {
  rollup "$1" --file `basename "$1" .js`.bundle.js --format es --plugin commonjs --plugin node-polyfills
}

build_cjs() {
  rollup "$1" --file `basename "$1" .js`.bundle.cjs --format cjs --plugin commonjs
}
```

### Usage

```zsh
build test.js
```

```zsh
build_cjs test.js
```
