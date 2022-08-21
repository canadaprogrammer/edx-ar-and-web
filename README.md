# Work with Augmented Reality (AR) and the Web

## More Complex Table Views

- Create a custom table view cell for different reasons:
  - to display more text, more buttons etc.
  - customize object locations within cells
- Custom View Creation: Steps Involved
  - Select the Cell
  - In the Attributes inspector set Style to Custom
  - Using Interface Builder tools, we can customize it
- Content Hugging
  - The flag needs to fit snugly into the content area
  - Change the horizontal field priority in Content Hugging Priority
  - From 251 to 252
  - Priorities the placement by the Auto Layout Engine
- New Cell SubClass
  - A custom table view class is needed
  - We can create outlets for configuring the cell
  - Ensure it is a Custom class of FlagTableViewCell
- Editing Table Views
  - In editing mode the table view calls the delegate method: `tableView(_: editingStyleForRowAt: )`
  - There are 3 options: `.none`, `.delete`, `.insert`
- Delegate Methods
  - Delegate methods are called in order in edit mode
    1. `tableView(_: canEditRowAt: )`
    2. `tableView(_: editingStyleRowAt: )`
    3. User does something here...
    4. `tableView(_: commit: forRowAt: )`
- Adding to the Flags
  - Add a + button to the navigation bar
  - Use a new view controller to add details
  - the same view controller for edits and additions can be used
  - A static Table View is used in this situation
- Static Table Views
  - Use a table view controller
  - Do NOT implement the data source protocol
  - Populate the table view using `viewDidLoad()`
- Add a Navigation Controller
- To the Navigation Controller
- Develop the Table View
  - Setting the content to Static Cells
  - Change the labels to reflect the content
- Saving Canceling
  - Add Navigation Bar items
  - Almost all Apps have these buttons: Save and Cancel
  - Save only when something changed

Moved this notes to [edx first ios app](https://github.com/canadaprogrammer/edx-first-ios-app#more-complex-table-views)
