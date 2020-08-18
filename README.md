# Rollup

This work is devoted to God.

## Installing

```sh
npm install --global rollup @rollup/plugin-commonjs rollup-plugin-node-polyfills
```

## Building

```sh
rollup main.js --file bundle.js --format es --plugin commonjs --plugin node-polyfills
```

## ZSH Function

```zsh
build() {
	rollup main.js --file bundle.js --format es --plugin commonjs --plugin node-polyfills
}
```

