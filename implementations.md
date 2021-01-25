---
layout: default
title: Implementations
banner: surprised.jpg
---
In this page you can find anonymous credentials schemes that have been
specified and implemented and hence we can get concrete performance figures out of them.

### Privacy Pass [\[PDF\]](https://www.petsymposium.org/2018/files/papers/issue3/popets-2018-0026.pdf)

- [Website](https://privacypass.github.io/)
- Source code: [Client](https://github.com/privacypass/challenge-bypass-extension) & [Server](https://github.com/privacypass/challenge-bypass-server)
- Properties: Strong-unlinkability, Single-show
- Based on: [(V)OPRF]({{site.baseurl}}/primitives.html#oprfs)
- Performance: TODO

### Signal Private Group System [\[PDF\]](https://eprint.iacr.org/2019/1416)

- [Implementation](https://github.com/signalapp/Signal-Android/tree/master/libsignal/service/src/main/java/org/whispersystems/signalservice/api/groupsv2)
- Properties: Multi-show, Public Attributes
- Based on: [KVAC]({{site.baseurl}}/primitives.html#kvac)
- Performance:
  - Credential Size: [493 bytes](https://youtu.be/4eKwlSqGUi4?list=PLeeS-3Ml-rpoVMNQkUrFDSfaTuUMxVtjy&t=2481)
  - Key size: TODO
  - Show size: TODO
  - Prover time: [2.16ms](https://youtu.be/4eKwlSqGUi4?list=PLeeS-3Ml-rpoVMNQkUrFDSfaTuUMxVtjy&t=2481)
  - Verifier time: [1.17ms](https://youtu.be/4eKwlSqGUi4?list=PLeeS-3Ml-rpoVMNQkUrFDSfaTuUMxVtjy&t=2481)

### Coconut [\[PDF\]](https://arxiv.org/pdf/1802.07344.pdf)

- [Implementation](https://github.com/asonnino/coconut) and [another implementation](https://gitlab.com/narodnik/darkwallet/-/tree/master/src/coconut)
- Properties: Threshold Issuance, Public/Private Attributes, Multi-show
- Based on: [PS signatures]({{site.baseurl}}/primitives.html#ps-signatures)
- Performance:
  - Credential Size: [132 bytes](https://sheharbano.com/assets/talks/talk_coconut.pdf)
  - Key size: TODO
  - Show size: [355 bytes](https://sheharbano.com/assets/talks/talk_coconut.pdf)
  - Prover time: [3.35 ms](https://sheharbano.com/assets/talks/talk_coconut.pdf)
  - Verifier time: [10.49 ms](https://sheharbano.com/assets/talks/talk_coconut.pdf)

### U-Prove [\[PDF\]](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/U-Prove20Cryptographic20Specification20V1.1.pdf)

- [U-Prove implementation](https://github.com/Microsoft/uprove-csharp-sdk)
- Properties: Single-show, Attributes
- Based on: TODO
- Performance: TODO

### Idemix [\[PDF\]](https://www.cise.ufl.edu/~nemo/anonymity/papers/idemix.pdf)

- [Implementation](prime.inf.tu-dresden.de/idemix/)
- Properties: Constant Credential Size, Multi-show
- Based on: [Blind RSA]({{site.baseurl}}/primitives.html#blind-rsa)
- Performance: TODO

[Idemix]: https://idemix.wordpress.com/

### [aeonflux]

- [aeonflux] Implementation
- Properties: Multi-show, Attributes
- Based on: [Algebraic MACs]({{site.baseurl}}/primitives.html#algebraic-macs)
- Performance: TODO

[aeonflux]: https://github.com/isislovecruft/aeonflux

### Facebook

https://engineering.fb.com/2019/10/16/security/partially-blind-signatures/
