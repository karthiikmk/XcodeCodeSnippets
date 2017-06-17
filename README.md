# XcodeCodeSnippets

  Hello world, Here i have wrote some useful snippets to get your most OFTEN code blocks easier. Hope this will help you to get the snippets on the fly.
 
# How to import all code snippets to Xcode

All Xcode code snippets exist as a .plist files in ~/Library/Developer/Xcode/UserData/CodeSnippets/ You can simply copy all code snippets (.codesnippet) into this folder, restart Xcode and you should have all of them ready to use.  

Note: Create the folder if it doesn't exist already. It is created by Xcode when user adds his first custom snippet.

# Snippets

swift-tableviewProtocols        To get tableview basic delegate and datasource methods in seperate extension

simply, type tableviewProtocol a popup will appear with the snippet {} symbol. 

```swift
extension <#UIViewController#>: UITableViewDelegate, UITableViewDataSource {
    
    func config() {
        
        //self.tableview.delegate = self
        //self.tableview.dataSource = self
        
        //self.tableview.clearEmptyCell()
    }
    
    func numberOfSections(in tableView: UITableView) -> Int {
        return <#sectionCount#>
    }
    
    func tableView(_ tableView: UITableView, numberOfRowsInSection section: Int) -> Int {
        return <#rowsCount#>
    }
    
    func tableView(_ tableView: UITableView, cellForRowAt indexPath: IndexPath) -> UITableViewCell {
        return <#UITableViewCell#>
    }
    
    func tableView(_ tableView: UITableView, didSelectRowAt indexPath: IndexPath) {
        tableView.deselectRow(at: indexPath, animated: true)
        <#code#>
    }
}
```

swift-mainQueue            To get mainQueue block

simply type main, a popup will appear with the snippet {} symbol. 

``` swift
DispatchQueue.main.async {
            
}
```

similarly, to get mark type "mark"

here you go

``` swift

// MARK: Details

``` 

Thanks, 
< karthik \>
