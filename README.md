# wasm-cra
Set up a create-react-app TypeScript project with WASM in a single step

## Overview
*Circa January 2021*

This script is based on [this](https://dev.to/techtrouts/embed-rust-wasm-into-react-48og) article by Carlos Ouro (August 2020).

It sets up a TypeScript create-react-app project with customize-cra/react-app-rewired such that a rust WASM libraries are set up to output wasm-pack output to the `src/` directory and with a WasmPackPlugin watcher. Please note that react-app-rewired "can break things" in terms of create-react-app guarantees.

## Prerequisites
* [npm](https://www.npmjs.com/get-npm)
* [cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html)

## Usage
`wasm-cra.py <project name> --dir <output directory> --wasm <module 1> --wasm <module 2> ...`
