# base32

base32 implemented in grain

## usage

```grain
import { encode, ZBase32, Base32Hex, Crockford, Base32 } from "./base32"

encode(ZBase32, "The quick brown fox jumps over the lazy dog.")

=> "ktwgkedtqiwsg43ycj3g675qrbug66bypj4s4hdurbzzc3m1rb4go3jyptozw6jyctzsqmo"
```

## encodings

* ZBase32: <http://philzimmermann.com/docs/human-oriented-base-32-encoding.txt>
* Base32 (RFC 3548, RFC 4648): <https://datatracker.ietf.org/doc/html/rfc3548>
* Base32Hex (RFC 4648): <https://datatracker.ietf.org/doc/html/rfc4648>
* Crockford: <https://www.crockford.com/base32.html>

## testing

I used <https://cryptii.com/pipes/z-base-32> for testing. You might want to have a play with that site. It's very informative.

```grain
grain base32.test.gr
```
