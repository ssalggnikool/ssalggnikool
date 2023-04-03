<img src="https://cdn.discordapp.com/emojis/1084310943296663613.gif?size=96&quality=lossless" width="100" alt="ball"> <img src="https://cdn.discordapp.com/emojis/1084310943296663613.gif?size=96&quality=lossless" width="100" alt="ball"> <img src="https://cdn.discordapp.com/emojis/1084310943296663613.gif?size=96&quality=lossless" width="100" alt="ball"> <img src="https://cdn.discordapp.com/emojis/1084310943296663613.gif?size=96&quality=lossless" width="100" alt="ball"> <img src="https://cdn.discordapp.com/emojis/1084310943296663613.gif?size=96&quality=lossless" width="100" alt="ball"> 

-----
```swift
import SwiftUI
import SDWebImageSwiftUI

public var oomf: [Person] = [
  Person(
    alias: "Flower",
    name: "[redacted]",
    age: "[redacted]",
    pronouns: ["first": "she/her", "second": "they/them"],
    icon: URL(string: "https://avatars.githubusercontent.com/u/97859147?v=4")!,
    role: "Known for contributions at org:palera1n",
    publicprojs: false,
    location: "United States",
    swiftKnowledge: true,
    objcKnowledge: false,
    markdownKnowledge: true,
    htmlKnowledge: true,
    designer: true,
    socials: ["twitter": "@flowerible", "discord": "flower#1116", "github": "flowerible"]
  )
]

for person in oomf {
  if person.alias == "Flower" {
    person.state = .girl
  } else {
    person.state = nil
  }
}
```
