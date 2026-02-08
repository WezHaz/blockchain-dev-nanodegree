# Project #1. Create Your Identity on Bitcoin Core

## Overview

This project proves identity ownership by signing a message with a Bitcoin address and verifying the signature. It demonstrates basic wallet control and message signing using Bitcoin Core.

## Submission artifacts

Wallet address:

```
1MPUSndUm6NGZqv3yekP5JrLUkY8pthm6j
```

Message:

```
1MPUSndUm6NGZqv3yekP5JrLUkY8pthm6j: Udacity rocks!
```

Message signature:

```
INGxvCUHJeaJOycxLo3k4nrKlqal8eVV8pP1UtZlZMlTM7Gv9BtQjo4bI54S2EP2p9+hPvvU15slVCQQsoI5JZM=
```

## How to reproduce (Bitcoin Core CLI)

Prerequisites:
- Bitcoin Core installed
- Wallet created and loaded
- `bitcoin-cli` available on your PATH

Steps:
1) Generate a new address:
   ```
   bitcoin-cli getnewaddress
   ```
2) Sign a message with the address:
   ```
   bitcoin-cli signmessage "<address>" "Udacity rocks!"
   ```
3) Verify the signature:
   ```
   bitcoin-cli verifymessage "<address>" "<signature>" "Udacity rocks!"
   ```

If the signature is valid, Bitcoin Core returns `true`.

## Notes

- The message includes the address to make ownership explicit.
- This is a standard proof-of-ownership flow used in many wallet verification processes.
