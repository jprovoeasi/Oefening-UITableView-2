# Exercise-UITableView-2

In this exercise you will make a combination of a **static** and **dynamic** UITableView.

## Tasks
1. Add a UITableViewController to the storyboard. This controller will display the status of your selection
  - Configure this UITableViewController as **static**.
  - Create 1 static cell in the storyboard.
  - Create and connect the necessay outlets. This only works for a **static** table!
2. Add another UITableViewController to the storyboard. This controller will serve to pick a color from a list.
  - Configure this UITableViewController as **dynamic**.
  - Create a prototype cell.
  - Create your own subclass of UITableViewCell and configure this as the custom class of your prototype cell.
  - Implement alle required methods of the UITableViewDataSource and UITableViewDelegate protocol.
  - Store all colors in the UITableViewController in a **(NSArray *)**.
3. Connect the 2 UITableViewControllers with a **show** segue.
  - The goal is to perform the segue upon clicking the row.
  - You can do this directly from the storyboard.
4. Create your very own delegate protocol so that whenever you select a color in the 2nd UITableViewController this color is passed to the 1st UITableViewController.
  - Define your delegate protocol in the 2nd UITableViewController.
  - Create a property for this delegate protocol in the 2nd UITableViewController.
  - Set this property equal to the 1st UITableViewController inside the method `prepareForSegue:sender:`.
5. Change the height of the cells dynamically. All that is required is to implement the correct method from the UITableViewDelegate protocol.
6. Add another UITableViewController to the storyboard. This controller will serve to pick a font from a list.
  - Go through the same steps you have done to setup the UITableViewController of the colors.
  - To retrieve all font family names there is a **class**method on `UIFont` called `familyNames`.
  - To retrieve all fonts from a family there is a **class**method on `UIFont` called `fontNamesForFamilyName:`.
  - To convert a font name into a UIFont there is a **class**method on `UIFont` called `fontWithName:size:`.
  - Store all fonts in a **(NSDictionary *)** so that each key is equal to the font family name and the value is equal to the array of fonts for that family name.
7. Round the corners of the UIView that displays the selected color.
  - *Tip: every UIView has a `layer` property.*
8. Add a UISearchBar to the UITableViewController to allow the user to search for fonts.
  - Add a UISearchBar to the UITableViewController in the storyboard as a header view.
  - Set the UITableViewController as the delegate of the UISearchBar.
  - Make sure the UITableViewController conforms to the UISearchBarDelegate protocol, this is done by adding `<UISearchBarDelegate>` behind the interface declaration.
  - Implement the required delegate methods from the UISearchbar to detect a change in the search text.
  - Filter the fonts based on the search text and reload the UITableView.

## Solutions
The solutions are available in the **oplossing** branch of this repository.
