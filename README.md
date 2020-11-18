# serde-error

```
cargo build --target wasm32-unknown-unknown --release
   Compiling serde-error v0.1.0 (/home/amiya/Documents/workspace/blockchain/test_serialize_error/contract)
error[E0277]: the trait bound `StatusMessage: near_sdk::serde::Serialize` is not satisfied
    --> src/lib.rs:14:1
     |
14   | #[near_bindgen]
     | ^^^^^^^^^^^^^^^ the trait `near_sdk::serde::Serialize` is not implemented for `StatusMessage`
     | 
    ::: /home/amiya/.cargo/registry/src/github.com-1ecc6299db9ec823/serde_json-1.0.59/src/ser.rs:2189:17
     |
2189 |     T: ?Sized + Serialize,
     |                 --------- required by this bound in `near_sdk::serde_json::to_vec`
     |
     = note: this error originates in an attribute macro (in Nightly builds, run with -Z macro-backtrace for more info)

error: aborting due to previous error

For more information about this error, try `rustc --explain E0277`.
error: could not compile `serde-error`.

To learn more, run the command again with --verbose.
```