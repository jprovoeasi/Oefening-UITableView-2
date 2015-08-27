# Oefening-UITableView-2

In deze oefening maak je een combinatie van een **static** en **dynamic** UITableView.

## Opgaves
1. Voeg een UITableViewController toe aan het storyboard. Deze zal de status van jouw selectie(s) weergeven.
  - Configureer deze UITableViewController als **static**.
  - Maak 1 statische cell in het storyboard.
  - Maak en connecteer de nodige outlets. Dit gaat enkel en alleen omdat het een **statische** tabel is!
2. Voeg nog een UITableViewController toe aan het storyboard. Deze zal dienen om een kleur te kiezen uit een lijst.
  - Configureer deze UITableViewController als **dynamic**.
  - Maak een prototype cell.
  - Maak je eigen subklasse van UITableViewCell en zet deze als de custom klasse van jouw prototype cell.
  - Implementeer alle nodige methodes van het UITableViewDataSource en UITableViewDelegate protocol.
  - Sla alle kleuren in de UITableViewController op in een **(NSArray *)**.
3. Verbind de 2 UITableViewControllers met een **show** segue.
  - De bedoeling is dat je de segue performt wanneer op de rij geklikt wordt.
  - Dit kan je volledig vanuit het storyboard doen.
4. Zet je eigen delegate protocol op zodat wanneer je een kleur selecteert in de 2e UITableViewController deze kleur wordt doorgegeven aan de 1e UITableViewController.
  - Definiëer je eigen delegate protocol in de 2e UITableViewController.
  - Maak een property aan voor jouw eigen delegate in de 2e UITableViewController.
  - Zet de delegate gelijk aan de 1e UITableViewController vanuit de `prepareForSegue:sender:` methode.
5. Verander de hoogte van de cellen dynamisch. Implementeer hiervoor de juiste UITableViewDelegate methode.
6. Voeg een nieuwe UITableViewController toe. Deze zal dienen om een font te kiezen uit een lijst.
  - Overloop dezelfde stappen dan je gedaan hebt om de UITableViewController van de kleuren op te zetten.
  - Om alle font family names te bekomen is er een **klasse**methode op `UIFont` genaamd `familyNames`.
  - Om alle fonts binnen een family te bekomen is er een **klasse**methode op `UIFont`genaamd `fontNamesForFamilyName:`.
  - Om een font name om te zetten in een UIFont is er een **klasse**methode op `UIFont` genaamd `fontWithName:size:`.
  - Sla alle fonts op in een **(NSDictionary *)** zodat elke key de font family name is en de waarde overeenkomt met de array van fonts.
7. Rond de UIView die de geselecteerde kleur weergeeft af.
  - *Tip: elke UIView heeft een `layer` property.*
8. Aan de UITableViewController gaan we een UISearchBar toevoegen om de gebruiken toe te laten te zoeken naar fonts.
  - Voeg vanuit het storyboard een UISearchBar toe als headerView aan de UITableViewController.
  - Zet de UITableViewController als de delegate van de UISearchBar.
  - Geef aan dat de UITableViewController het protocol UISearchBarDelegate implementeert, dit doe je door `<UISearchBarDelegate>` toe te voegen achter de interface declaratie.
  - Implementeer de nodige delegate methode van de UISearchbar om te zoeken naar een font. Dit werkt door het model te filteren op basis van de zoaktekst en UITableView te reloaden.

## Oplossing
De oplossingen vind je terug onder de repository **Demo-UITableView**.
