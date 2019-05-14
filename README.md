# Advance Swift Cheatsheet
Working with Swift like pro <3 

### Group all related contants into `enum` over `struct`/`class`
```swift
enum Math {
  static let e = 2.718281828459045235360287
  static let root2 = 1.41421356237309504880168872
}
```
> The advantage of using a case-less enumeration is that it can't accidentally be instantiated and works as a pure namespace.

