# Axe Programming Language

Axe is a statically typed, compiled programming language that centred around ease of concurrency and memory safety. It is designed to be simple and easy to learn. 

## Requirements

For full LSP support, you need the Axe LSP server (`axe-lsp` or `axe-lsp.exe`) installed:

1. Build from source: `cd tooling/axe-lsp && ../../axe lsp_server.axe -o axe-lsp`
2. Place in your PATH, or configure the path in settings

## Extension Settings

This extension contributes the following settings:

* `axe.lsp.serverPath`: Path to the Axe LSP server executable
* `axe.lsp.trace`: Set to 'messages' or 'verbose' to debug LSP communication

## Example

```axe
use std.io;

def some_function() {
    println "Hello, world.";
}

def main() {
    some_function();
}
```

## Release Notes

### 0.0.10

- Added Language Server Protocol support
- Integrated LSP client for code intelligence
- Improved syntax highlighting

### 0.0.9

- Initial release with syntax highlighting
