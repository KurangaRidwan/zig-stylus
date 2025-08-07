**Zig File Descriptions**

account.zig
Retrieves the balance of a given address and outputs it using WebAssembly allocator and host I/O functions.

build.zig
Configures the build process for a WebAssembly executable, targeting wasm32-freestanding, linking C/C++ libraries, and setting up the user entrypoint.

chainid.zig
Fetches the blockchain chain ID using host I/O and outputs it as a 4-element u64 array.

counter.zig
Implements a persistent counter in storage, initializing it to 1 if unset, incrementing it otherwise, and outputting the current value.

entrypoint.zig
Defines a WebAssembly entrypoint that reads arguments, calls a user-defined main function, and outputs the result.

evmgas.zig
Retrieves the remaining EVM gas and outputs it as a 4-element u64 array.

main.zig
Stores and retrieves a string ("ola") under a key ("hello123") in storage, then outputs the retrieved value.

sender.zig
Emits a log event and outputs a 32-byte data array using host I/O functions.

storage.zig
Stores and retrieves a string ("ola") under a key ("hello123") in storage, then outputs the retrieved value (similar to main.zig).

WasmAllocator.zig
Implements a custom WebAssembly memory allocator with size-classed memory management, supporting allocation, resizing, and freeing of memory blocks.


**Summary:**  
Forked the zig-stylus repo, documented the what the files do