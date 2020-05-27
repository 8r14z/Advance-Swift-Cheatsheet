# Advanced Swift Cheatsheet
Working with Swift like pro <3 

### 1. Group all related contants into `enum` over `struct`/`class`
```swift
enum Math {
  static let e = 2.718281828459045235360287
  static let root2 = 1.41421356237309504880168872
}
```
> The advantage of using a case-less enumeration is that it can't accidentally be instantiated and works as a pure namespace.

### 2. Decode image in background thread
> [UIImage Decoding](https://github.com/HoaiAn1/UIImage-JPEGDecoding)

Image should be decoded before setting to UIImageView. `imageView.image = image` this call is running on main thread and under the hood it decodes the image

### 3. Enum should have raw value when using it as placeholder in string
Without this rawValue, it's using [Mirror](https://developer.apple.com/documentation/swift/mirror) to generate string from enum value. And Mirror operation is expensive. 

### 4. Class instances are expensive - Structs are cheap
Need to alocate head and heap alogirthnm is expensive
