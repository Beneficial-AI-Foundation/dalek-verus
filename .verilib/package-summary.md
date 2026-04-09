# Package Summary

This library provides implementations for a field of scalars, a group of curve points, and scalar multiplication operations over these structures. The set of scalars and the group are large enough to offer cryptographic security, and therefore require specialized implementations.

In addition, the library allows bitstring conversions to and from the algebraic structures, as well as conversions between equivalent forms of the elliptic curve group. Each form (Edwards, Montgomery, Ristretto) offers specific computational advantages for cryptographic operations.

Formal verification targets version 4.1.3 of the curve25519-dalek crate -- the version used by libsignal -- together with the Lizard extension introduced in Signal's fork of Dalek. Among the supported computational backends, only the serial u64 backend falls within the current verification scope.

## Applications

- Scalars can be used in protocols to store private keys and cryptographically secure random numbers.
- Curve points can be used to represent public keys or encode private data in a secure way.
- Scalar multiplication is used for multiple cryptographic operations, such as encoding, decoding, shared key generation, zero-knowledge proofs, private-key signing and verification.

