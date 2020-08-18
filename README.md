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
	rollup main.js --file bundle.js --format es --plugin commonjs --plugin node-polyfills
}
```

