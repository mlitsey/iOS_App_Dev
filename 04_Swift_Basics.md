# Swift Programming Basics
Collections, Constants & Variables  

## clone git repo

- from start page choose `clone a git repository`
- or from menu bar choose `Integrate` then `clone...`

```zsh
# cli method
git clone git@github.com:appbrewery/Dicee-iOS13.git
```

edit code in `ViewController.swift`

Select `Main.storyboard` then open the Assistant view to show side by side. 

hold control then click and drag the line to land between `class ViewController` and `override func`  
An options window will  then pop up.  
- name: (diceImageView1)
- connect

to see the underlying code of the `Main.storyboard`  
- right click `Main.storyboard`
- Open As
- Source Code

renaming an item should be done by
- right click the name (diceImageView1)
- Refactor
- Rename...
- (diceImageViewOne) click rename

set image to DiceSix
```swift
diceImageViewOne.image = UIImage(imageLiteralResourceName: "DiceSix")
```

comments are created using `//` followed by the comment  
comment block are created using `/*` to open and `*/` to close  

```swift
// single line comment
/* block or multi-line
comment
goes here
*/
diceImageViewOne.image = UIImage(imageLiteralResourceName: "DiceFour")
```

## 38 Respond to user interaction with IBActions

ctrl click drag to below the `ViewController` code block but above the final `}` brace.  
- Connection (Action)
- Object (View Controller)
- Name (rollButtonPressed)
- Type (UIButton)
- Event (Touch Up Inside)  
    - this is a tap
- Arguments (Sender)

The code added is 
```swift
@IBAction func rollButtonPressed(_ sender: UIButton) {
    }
```

## 44 random numbers

Random number from 1 to 6
`Int.random(in: 1...6)`

exclude the last number using `<`
`Int.random(in: 1..<6)`

Get a random element from an array
`array.randomElement()!`

or shuffle the items with in the array
`array.shuffle()`

