# Swift String Methods and Properties

## Initialization
- `init()`
- `init(repeating: Character, count: Int)`
- `init(repeating: String, count: Int)`
- `init(Character)`
- `init(CharacterView)`
- `init(Substring)`
- `init(Substring.UnicodeScalarView)`

## Properties
- `var isEmpty: Bool`
- `var count: Int`
- `var startIndex: String.Index`
- `var endIndex: String.Index`
- `var first: Character?`
- `var last: Character?`
- `var utf8: String.UTF8View`
- `var utf16: String.UTF16View`
- `var unicodeScalars: String.UnicodeScalarView`
- `var indices: String.Indices`

## Subscripts
- `subscript(index: String.Index) -> Character`
- `subscript(bounds: Range<String.Index>) -> Substring`
- `subscript(bounds: ClosedRange<String.Index>) -> Substring`

## Instance Methods
- `func hasPrefix(String) -> Bool`
- `func hasSuffix(String) -> Bool`
- `func lowercased() -> String`
- `func uppercased() -> String`
- `func capitalized() -> String`
- `func filter((Character) -> Bool) -> String`
- `func map<T>((Character) -> T) -> [T]`
- `func split(separator: Character, omittingEmptySubsequences: Bool = true) -> [Substring]`
- `func split(maxSplits: Int, omittingEmptySubsequences: Bool = true, whereSeparator: (Character) -> Bool) -> [Substring]`
- `func appending(String) -> String`
- `func contains(String) -> Bool`
- `func contains(Character) -> Bool`
- `func contains(where: (Character) -> Bool) -> Bool`
- `func prefix(Int) -> Substring`
- `func suffix(Int) -> Substring`
- `func dropFirst(Int) -> Substring`
- `func dropLast(Int) -> Substring`
- `func drop(while: (Character) -> Bool) -> Substring`
- `func trimmingCharacters(in: CharacterSet) -> String`
- `func replacingOccurrences(of: String, with: String) -> String`
- `func replacingOccurrences(of: String, with: String, options: NSString.CompareOptions = [], range: Range<String.Index>? = nil) -> String`
- `func replacingOccurrences<Target, Replacement>(of target: Target, with replacement: Replacement) -> String where Target: StringProtocol, Replacement: StringProtocol`
- `func padding(toLength: Int, withPad: String, startingAt: Int) -> String`
- `func index(before: String.Index) -> String.Index`
- `func index(after: String.Index) -> String.Index`
- `func index(String.Index, offsetBy: Int) -> String.Index`
- `func index(String.Index, offsetBy: Int, limitedBy: String.Index) -> String.Index?`
- `func distance(from: String.Index, to: String.Index) -> Int`

## Static Methods
- `static func localizedStringWithFormat(String, CVarArg...) -> String`

## Comparison Methods
- `func compare(String) -> ComparisonResult`
- `func compare(String, options: NSString.CompareOptions) -> ComparisonResult`
- `func localizedCompare(String) -> ComparisonResult`
- `func caseInsensitiveCompare(String) -> ComparisonResult`

## Foundation Extensions
- `func data(using: String.Encoding) -> Data?`
- `func data(using: String.Encoding, allowLossyConversion: Bool) -> Data?`
- `func range(of: String) -> Range<String.Index>?`
- `func range(of: String, options: NSString.CompareOptions, range: Range<String.Index>?, locale: Locale?) -> Range<String.Index>?`
