# What is `SwiftBootstring`?

`SwiftBootstring` is an implementaion of [Bootstring](https://tools.ietf.org/html/rfc3492) in [Swift](https://swift.org/).
It was originally written as a part of [SwiftCGIResponder](https://github.com/YOCKOW/SwiftCGIResponder).


## What is `Bootstring`?

Bootstring is a string encoding methods.  
One of instances of Bootstring is Punycode, that is used to encode  internationalized domain name(IDN).
Please refer to [RFC 3492](https://tools.ietf.org/html/rfc3492) for details.


# Requirements

## Swift

- Swift 6*
- Swift 5*

(* including language mode of Swift 5, 4.2, or 4)

## OS

- macOS
- Ubuntu


# Usage

```
import Bootstring

print("MajiでKoiする5秒前".addingPunycodeEncoding!)
// -> MajiKoi5-783gue6qz075azm5e

print("3B-ww4c5e180e575a65lsy2b".removingPunycodeEncoding!)
// -> 3年B組金八先生
```


# License

MIT License.  
See "LICENSE.txt" for more information.
